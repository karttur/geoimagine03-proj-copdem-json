---
layout: article
title: 0001_CreatesScaling_DEM_v090.json
categories: projects
excerpt: \# Create scaling for fitting DEM data to byte range
tags:: 
    - 0001_CreatesScaling_DEM
date: 2021-12-19
modified: 2021-12-19
comments: true
share: true
---

# 0001 CreatesScaling DEM (projects)

### \# Create scaling for fitting DEM data to byte range

The json command file <span class='file'>0001_CreatesScaling_DEM_v090.json</span> is part of karttur's GeoImagine project <span class='project'>projects</span>. Calling the json file will execute the following commands of the GeoImagine Framework.

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
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 0.03125,
        "mirror0": false
      },
      "comp": [
        {
          "dem": {
            "source": "*",
            "product": "*",
            "content": "dem",
            "layerid": "dem",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 1,
        "mirror0": false
      },
      "comp": [
        {
          "dem": {
            "source": "*",
            "product": "*",
            "content": "dem",
            "layerid": "dem1",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 4,
        "mirror0": false
      },
      "comp": [
        {
          "slope": {
            "source": "*",
            "product": "*",
            "content": "dem",
            "layerid": "slope",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 1,
        "mirror0": true
      },
      "comp": [
        {
          "shade": {
            "source": "*",
            "product": "*",
            "content": "dem",
            "layerid": "shade",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": true,
      "parameters": {
        "scalefac": 5,
        "mirror0": true
      },
      "comp": [
        {
          "tpi": {
            "source": "*",
            "product": "*",
            "content": "dem",
            "layerid": "tpi",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": true,
      "parameters": {
        "scalefac": 5,
        "mirror0": false
      },
      "comp": [
        {
          "tri": {
            "source": "*",
            "product": "*",
            "content": "dem",
            "layerid": "tri",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 50000,
        "mirror0": true
      },
      "comp": [
        {
          "profc": {
            "source": "*",
            "product": "*",
            "content": "dem",
            "layerid": "profc",
            "suffix": "*"
          }
        },
        {
          "crosc": {
            "source": "*",
            "product": "*",
            "content": "dem",
            "layerid": "crosc",
            "suffix": "*"
          }
        },
        {
          "longc": {
            "source": "*",
            "product": "*",
            "content": "dem",
            "layerid": "longc",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 1000,
        "mirror0": true
      },
      "comp": [
        {
          "planc": {
            "source": "*",
            "product": "*",
            "content": "dem",
            "layerid": "planc",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 25,
        "mirror0": false
      },
      "comp": [
        {
          "rusle-slopelength": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "rusle-slopelength",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 50,
        "offsetadd": -2,
        "mirror0": false
      },
      "comp": [
        {
          "rusle-slopesteepness": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "rusle-slopesteepness",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 2,
        "offsetadd": 25,
        "mirror0": false
      },
      "comp": [
        {
          "near-divide-head": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "near-divide-head",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 2,
        "offsetadd": 25,
        "mirror0": false
      },
      "comp": [
        {
          "far-divide-head": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "far-divide-head",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 2,
        "offsetadd": 25,
        "mirror0": false
      },
      "comp": [
        {
          "near-divide-head": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "near-divide-head",
            "suffix": "*"
          },
          "far-divide-head": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "far-divide-head",
            "suffix": "*"
          },
          "hydraulhead": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "hydraulhead",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 0.05555,
        "mirror0": false
      },
      "comp": [
        {
          "stream-dist": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "stream-dist",
            "suffix": "v01-pfpf-hydrdem4+4-90m"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 0.1111,
        "mirror0": false
      },
      "comp": [
        {
          "near-divide-dist": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "near-divide-dist",
            "suffix": "v01-pfpf-hydrdem4+4-90m"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 0.01111,
        "mirror0": false
      },
      "comp": [
        {
          "far-divide-dist": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "far-divide-dist",
            "suffix": "v01-pfpf-hydrdem4+4-90m"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 12,
        "log": true,
        "mirror0": false
      },
      "comp": [
        {
          "sfd-updrain": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "sfd-updrain",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 12,
        "log": true,
        "mirror0": false
      },
      "comp": [
        {
          "mfd-updrain": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "mfd-updrain",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 20,
        "log": true,
        "mirror0": false
      },
      "comp": [
        {
          "psi": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "psi",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 20,
        "log": true,
        "mirror0": false
      },
      "comp": [
        {
          "spi": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "spi",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 10,
        "offsetadd": -30,
        "mirror0": false
      },
      "comp": [
        {
          "tci": {
            "source": "*",
            "product": "*",
            "content": "terrain",
            "layerid": "tci",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": false,
      "parameters": {
        "scalefac": 1,
        "mirror0": false
      },
      "comp": [
        {
          "lftpi": {
            "source": "*",
            "product": "*",
            "content": "dem",
            "layerid": "landform-tpi",
            "suffix": "*"
          }
        },
        {
          "landform-ps": {
            "source": "*",
            "product": "*",
            "content": "dem",
            "layerid": "landform-ps",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": true,
      "parameters": {
        "scalefac": 10,
        "mirror0": false
      },
      "comp": [
        {
          "lfgeomrph": {
            "source": "*",
            "product": "*",
            "content": "dem",
            "layerid": "geomorph",
            "suffix": "*"
          }
        }
      ]
    },
    {
      "processid": "CreateScaling",
      "overwrite": true,
      "parameters": {
        "scalefac": 10,
        "mirror0": false
      },
      "comp": [
        {
          "landform-ps": {
            "source": "*",
            "product": "*",
            "content": "dem",
            "layerid": "landform-ps",
            "suffix": "*"
          }
        }
      ]
    }
  ]
}
```
