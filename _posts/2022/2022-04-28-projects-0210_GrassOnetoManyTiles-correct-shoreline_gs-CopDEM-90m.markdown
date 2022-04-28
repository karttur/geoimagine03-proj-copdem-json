---
layout: article
title: 0210_GrassOnetoManyTiles-correct-shoreline_gs-CopDEM-90m.json
categories: copdem90gs
excerpt:  Correct the CopDEM 90m shoreline
tags:: 
    - 0210_GrassOnetoManyTiles-correct-shoreline_gs-CopDEM-90m
date: 2022-04-28
modified: 2022-04-28
comments: true
share: true
---

# 0210 GrassOnetoManyTiles correct shoreline gs CopDEM 90m (projects)

##  Correct the CopDEM 90m shoreline

The json command file <span class='file'>0210_GrassOnetoManyTiles-correct-shoreline_gs-CopDEM-90m.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

```
{
  "userproject": {
    "userid": "karttur",
    "projectid": "karttur-northlandease2n",
    "tractid": "karttur-northlandease2n",
    "siteid": "*",
    "plotid": "*",
    "system": "ease2n"
  },
  "period": {
    "timestep": "static"
  },
  "process": [
    {
      "processid": "GrassOnetoManyTiles",
      "version": "1.3",
      "overwrite": true,
      "dryrun": false,
      "verbose": 1,
      "parameters": {
        "regionlayer": "DEM",
        "asscript": true,
        "mosaic": true,
        "subparameter": [
          {
            "r.in.gdal": {
              "flags": "e",
              "input": "srcFPN",
              "output": "DEM"
            }
          },

          {
            "g.region": {
              "raster": "DEM"
            }
          },
          {
            "r.mapcalc": {
              "\"landDEM ": " if((DEM==0),null(),DEM)\"",
              "overwrite": true
            }
          },
          {
            "null": {
              "data":"\"$(r.stats -p input=landDEM null_value='null')\""
            }
          },
          {
            "null": {
              "null": "if echo \"$data\" | grep -q \"null\"; then"
            }
          },
          {
            "null": {
              "null": "echo \"Coastline tile\""
            }
          },
          {
            "r.mapcalc": {
              "\"drain_terminal ": " if((DEM==0),1,null())\"",
              "overwrite": true
            }
          },
          {
            "r.clump": {
              "input": "drain_terminal",
              "output": "terminal_clumps",
              "overwrite": true
            }
          },
          {
            "r.to.vect": {
              "input": "terminal_clumps",
              "output": "terminal_clumps",
              "type": "area",
              "overwrite": true
            }
          },
          {
            "v.to.db": {
              "map": "terminal_clumps",
              "type": "centroid",
              "option": "area",
              "columns": "area_km2",
              "units": "kilometers",
              "overwrite": true
            }
          },
          {
            "v.out.ogr": {
              "input": "terminal_clumps",
              "type": "area",
              "format": "ESRI_Shapefile",
              "output": "terminal_clumps-out",
              "overwrite": true
            }
          },
          {
            "v.to.rast": {
              "input": "terminal_clumps",
              "type": "area",
              "where": "\"area_km2< 5.0\"",
              "output": "drain_terminal_small",
              "use": "val",
              "value": 0,
              "overwrite": true
            }
          },
          {
            "v.to.rast": {
              "input": "terminal_clumps",
              "type": "area",
              "where": "\"area_km2>= 5.0\"",
              "output": "drain_terminal_large",
              "use": "val",
              "value": 0,
              "overwrite": true
            }
          },

          {
            "r.mapcalc": {
              "\"land ": " if(( isnull(drain_terminal_large)), 1 ,null())\"",
              "overwrite": true
            }
          },
          {
            "r.buffer": {
              "input": "drain_terminal_large",
              "output": "shorep1",
              "distance": 128.56,
              "units": "meter",
              "overwrite": true
            }
          },
          {
            "r.mapcalc": {
              "\"shoreline_ini ": " if((shorep1>0 && land==1),1,null())\"",
              "overwrite": true
            }
          },
          {
            "r.mapcalc": {
              "\"negative_DEM ": " if((DEM<0),0,null())\"",
              "overwrite": true
            }
          },
          {
            "r.mapcalc": {
              "\"negativeshoreline_DEM ": " if((DEM<0 && shoreline_ini >0),1,null())\"",
              "overwrite": true
            }
          },
          {
            "r.cost": {
              "flags": "n",
              "input": "negative_DEM",
              "output": "sea_pits",
              "start_raster": "negativeshoreline_DEM",
              "max_cost": 0,
              "overwrite": true
            }
          },
          {
            "r.mapcalc": {
              "\"inland_comp_DEM ": " if(( isnull(sea_pits) ), if((isnull(land)), null(),DEM) , null())\"",
              "overwrite": true
            }
          },
          {
            "r.mapcalc": {
              "\"terminal_drain ": " if((isnull (inland_comp_DEM)),1,null())\"",
              "overwrite": true
            }
          },
          {
            "r.buffer": {
              "input": "terminal_drain",
              "output": "shorep1",
              "distance": 128.56,
              "units": "meter",
              "overwrite": true
            }
          },
          {
            "r.mapcalc": {
              "\"shoreline ": " if((shorep1>0 && inland_comp_DEM>=0),1,null())\"",
              "overwrite": true
            }
          },
          {
            "null": {
              "null": "else"
            }
          },
          {
            "r.mapcalc": {
              "\"inland_comp_DEM ": " landDEM\"",
              "overwrite": true
            }
          },
          {
            "null": {
              "null": "fi"
            }
          },
          {
            "r.out.gdal": {
              "input": "inland_comp_DEM",
              "output": "inland_comp_DEM-out",
              "overwrite": true
            }
          }
        ]
      },
      "srcpath": {
        "volume": "Ancillary",
        "hdr": "tif"
      },
      "dstpath": {
        "volume": "Ancillary",
        "hdr": "tif"
      },
      "srccomp": [
        {
          "*": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "copdem",
            "prefix": "dem",
            "suffix": "v01-pfpf-hydrdem4+4-90m"
          }
        }
      ],
      "dstcopy": [
        {
          "terminal_clumps-out": {
            "source": "copy",
            "product": "copy",
            "content": "terminal-polys",
            "layerid": "terminal-polys",
            "prefix": "terminal-polys",
            "suffix": "v01-pfpf-hydrdem4+4-90m",
            "ext": ".shp"
          }
        },
        {
          "inland_comp_DEM-out": {
            "source": "copy",
            "product": "copy",
            "content": "landdem",
            "layerid": "land-dem",
            "prefix": "land-dem",
            "suffix": "v01-pfpf-hydrdem4+4-90m"
          }
        }
      ]
    }
  ]
}
```
