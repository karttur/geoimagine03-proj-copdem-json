---
layout: article
title: 0003_createlegends_DEM_v090.json
categories: common
excerpt:  Create legend for byte range DEM data
tags:: 
    - 0003_createlegends_DEM
date: 2022-04-28
modified: 2022-04-28
comments: true
share: true
---

# 0003 createlegends DEM (projects)

##  Create legend for byte range DEM data

The json command file <span class='file'>0003_createlegends_DEM_v090.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

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
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Elevation (m.a.s.l)",
        "precision": "0"
      },
      "srccomp": [
        {
          "dem1": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "dem1",
            "prefix": "dem1",
            "suffix": "v01-90m"
          }
        }
      ]
    },

    {
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Slope steepness (degrees)",
        "precision": "0"
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
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Profile curvature",
        "precision": "0"
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
        }
      ]
    },
    {
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Plan curvature",
        "precision": "0"
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
        }
      ]
    },
    {
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Longitudinal curvature",
        "precision": "0"
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
        }
      ]
    },
    {
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "cross-sectional curvature",
        "precision": "0"
      },
      "srccomp": [
        {
          "profc3": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "crosc",
            "prefix": "crosc",
            "suffix": "v01-90m-grass-3x3"
          }
        }
      ]
    },
    {
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Topographic Ruggedness Index",
        "precision": "0"
      },
      "srccomp": [
        {
          "tri3": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "tri",
            "prefix": "tri",
            "suffix": "*"
          }
        }
      ]
    },

    {
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Topographic Position Index",
        "precision": "0"
      },
      "srccomp": [
        {
          "tpi3": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "tpi",
            "prefix": "tpi",
            "suffix": "*"
          }
        }
      ]
    },

    {
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Topographic Ruggedness Index",
        "precision": "0"
      },
      "srccomp": [
        {
          "tri3": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "tri",
            "prefix": "tri",
            "suffix": "*"
          }
        }
      ]
    },

    {
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Landform (from TPI)",
        "precision": "0"
      },
      "srccomp": [
        {
          "lftpi": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "landform-tpi",
            "prefix": "landform-tpi",
            "suffix": "*"
          }
        }
      ]
    },

    {
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Landform (geomorphon)",
        "precision": "0"
      },
      "srccomp": [
        {
          "geomorph": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "geomorph",
            "prefix": "geomorph",
            "suffix": "*"
          }
        }
      ]
    },

    {
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Landform (curvature)",
        "precision": "0"
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
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Updrain area (km2)",
        "precision": "0"
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
        }
      ]
    },
    {
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Updrain area (km2)",
        "precision": "0"
      },
      "srccomp": [
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
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Proximity (km)",
        "precision": "0"
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
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Proximity (km)",
        "precision": "0"
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
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Proximity (km)",
        "precision": "0"
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
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Hydraulic head (m)",
        "precision": "0"
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
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Vertical head (m)",
        "precision": "0"
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
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Vertical head (m)",
        "precision": "0"
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
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "StreamPoiwer Index (SPI)",
        "precision": "0"
      },
      "srccomp": [
        {
          "spi": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "spi",
            "prefix": "spi",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "RUSLE L factor",
        "precision": "0"
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
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "RUSLE S factor",
        "precision": "0"
      },
      "srccomp": [
        {
          "terrain_slopesteepness": {
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
      "processid": "CreateLegend",
      "overwrite": false,
      "parameters": {
        "columnhead": "Topographic Convergence Index (TCI)",
        "precision": "0"
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
    }
  ]
}
```
