---
layout: article
title: 0005_exportlegend_DEM_v090.json
categories: common
excerpt:  Export legend for DEM data
tags:: 
    - 0005_exportlegend_DEM
date: 2022-10-05
modified: 2022-10-05
comments: true
share: true
---

# 0005 exportlegend DEM (projects)

##  Export legend for DEM data

The json command file <span class='file'>0005_exportlegend_DEM_v090.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

```
{
  "userproject": {
    "userid": "karttur",
    "projectid": "karttur",
    "tractid": "karttur",
    "siteid": "*",
    "plotid": "*",
    "system": "system"
  },
  "period": {
    "timestep": "static"
  },
  "process": [
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "dem_darkest_fixed",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "dem": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "dem1",
            "prefix": "dem-darkest",
            "suffix": "v01-90m"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "dem_dark_fixed",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "dem": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "dem1",
            "prefix": "dem-dark",
            "suffix": "v01-90m"
          }
        }
      ]
    },

    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "dem_light_fixed",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "dem": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "dem1",
            "prefix": "dem-light",
            "suffix": "v01-90m"
          }
        }
      ]
    },

    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "dem_lightest_fixed",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "dem": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "dem1",
            "prefix": "dem-lightest",
            "suffix": "v01-90m"
          }
        }
      ]
    },

    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "slope",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "slope": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "slope",
            "prefix": "slope",
            "suffix": "v01-90m-grass-3x3"
          }
        }
      ]
    },

    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "slope2",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "slope": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "slope",
            "prefix": "slope",
            "suffix": "v01-90m-grass-3x3"
          }
        }
      ]
    },

    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "slope3",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "slope": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "slope",
            "prefix": "slope",
            "suffix": "v01-90m-grass-3x3"
          }
        }
      ]
    },

    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "demcurvature",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "profc3": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "profc",
            "prefix": "profc",
            "suffix": "v01-90m-grass-3x3"
          }
        },
        {
          "profc9": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "profc",
            "prefix": "profc",
            "suffix": "v01-90m-grass-9x9"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "demcurvature",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "crosc3": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "crosc",
            "prefix": "crosc",
            "suffix": "v01-90m-grass-3x3"
          }
        },
        {
          "crosc9": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "crosc",
            "prefix": "crosc",
            "suffix": "v01-90m-grass-9x9"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "demcurvature",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "planc3": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "planc",
            "prefix": "planc",
            "suffix": "v01-90m-grass-3x3"
          }
        },
        {
          "planc9": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "planc",
            "prefix": "planc",
            "suffix": "v01-90m-grass-9x9"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "demcurvature",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "longc3": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "longc",
            "prefix": "longc",
            "suffix": "v01-90m-grass-3x3"
          }
        },
        {
          "longc9": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "longc",
            "prefix": "longc",
            "suffix": "v01-90m-grass-9x9"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "tri",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "tri3": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "tri",
            "prefix": "tri",
            "suffix": "v01-90m-3x3"
          }
        },
        {
          "tri9": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "tri",
            "prefix": "tri",
            "suffix": "v01-90m-9x9"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "tri2",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "tri3": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "tri",
            "prefix": "tri",
            "suffix": "v01-90m-3x3"
          }
        },
        {
          "tri9": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "tri",
            "prefix": "tri",
            "suffix": "v01-90m-9x9"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "tpi",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "tpi3": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "tpi",
            "prefix": "tpi",
            "suffix": "v01-90m-3x3"
          }
        },
        {
          "tpi9": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "tpi",
            "prefix": "tpi",
            "suffix": "v01-90m-9x9"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "tri",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "tri3": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "tri",
            "prefix": "tri",
            "suffix": "v01-90m-3x3"
          }
        },
        {
          "tri9": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "tri",
            "prefix": "tri",
            "suffix": "v01-90m-9x9"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "landformTPIdouble",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "lftpi": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "landform-tpi",
            "prefix": "landform-tpi",
            "suffix": "v01-90m-np-stnd-1+3"
          }
        }
      ]
    },

    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "landformTPI",
        "legendnominal":false,
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "lftpi": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "landform-tpi",
            "prefix": "landform-tpi",
            "suffix": "v01-90m-np-stnd-1+3"
          }
        }
      ]
    },

    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "geomorphlegend",
        "legendnominal":false,
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "lftpi": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "geomorph",
            "prefix": "geomorph",
            "suffix": "v01-90m-grass-3x3"
          }
        }
      ]
    },



    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "ps-morphology-legend",
        "legendnominal":false,
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "landform-ps": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "landform-ps",
            "prefix": "landform-ps",
            "suffix": "*"
          }
        }
      ]
    },




    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "updrain",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "mfd-updrain": {
            "source": "ESA",
            "product": "copdem",
            "content": "terrain",
            "layerid": "mfd-updrain",
            "prefix": "mfd-updrain",
            "suffix": "v01-pfpf-hydrdem4+4-90m"
          }
        },
        {
          "sfd-updrain": {
            "source": "ESA",
            "product": "copdem",
            "content": "terrain",
            "layerid": "sfd-updrain",
            "prefix": "sfd-updrain",
            "suffix": "v01-pfpf-hydrdem4+4-90m"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "invgeneralproximity",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "stream-dist": {
            "source": "ESA",
            "product": "copdem",
            "content": "terrain",
            "layerid": "stream-dist",
            "prefix": "stream-dist",
            "suffix": "v01-pfpf-hydrdem4+4-90m"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "streamproximity",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "stream-dist": {
            "source": "ESA",
            "product": "copdem",
            "content": "terrain",
            "layerid": "stream-dist",
            "prefix": "stream-dist",
            "suffix": "v01-pfpf-hydrdem4+4-90m"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "far-divide-dist",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "far-divide-dist": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "far-divide-dist",
            "prefix": "far-divide-dist",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "dividehead",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "far-divide-head": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "far-divide-head",
            "prefix": "far-divide-head",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "dividehead",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "near-divide-head": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "near-divide-head",
            "prefix": "near-divide-head",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "hydraulhead",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "far-divide-head": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "near-divide-head",
            "prefix": "near-divide-head",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "near-divide-dist",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "near-divide-dist": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "near-divide-dist",
            "prefix": "near-divide-dist",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "hydraulhead",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "hydraulhead": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "hydraulhead",
            "prefix": "hydraulhead",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "ruslelfactor",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "terrain_rusle-slopelength": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "rusle-slopelength",
            "prefix": "rusle-slopelength",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "ruslesfactor",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "terrain_rusle-slopesteepness": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "rusle-slopesteepness",
            "prefix": "rusle-slopesteepness",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "tci",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "terrain_tci": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "tci",
            "prefix": "tci",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "ExportLegend",
      "overwrite": false,
      "parameters": {
        "palette": "spi",
        "legendopacity": 128
      },
      "dstpath": {
        "volume": "GeoImg2021"
      },
      "srccomp": [
        {
          "terrain_spi": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "spi",
            "prefix": "spi",
            "suffix": "*"
          }
        }
      ]
    }
  ]
}
```
