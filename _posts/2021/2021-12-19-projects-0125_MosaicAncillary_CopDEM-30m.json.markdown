---
layout: article
title: 0125_MosaicAncillary_CopDEM-30m.json
categories: projects
excerpt: \# Import the CopDEM 30 m virtual data to the Framework
tags:: 
    - 0125_MosaicAncillary_CopDEM-30m.json
date: 2021-12-19
modified: 2021-12-19
comments: true
share: true
---

# 0125 MosaicAncillary CopDEM 30m.json (projects)

### \# Import the CopDEM 30 m virtual data to the Framework

The json command file <span class='file'>0125_MosaicAncillary_CopDEM-30m.json</span> is part of karttur's GeoImagine project <span class='project'>projects</span>. Calling the json file will execute the following commands of the GeoImagine Framework.

```
{
  "userproject": {
    "userid": "karttur",
    "projectid": "karttur",
    "tractid": "karttur",
    "siteid": "*",
    "plotid": "*",
    "system": "ancillary"
  },
  "period": {
    "timestep": "static"
  },
  "process": [
    {
      "processid": "MosaicAncillary",
      "overwrite": false,
      "parameters": {
        "mosaiccode": "subdirfiles",
        "datadir": "/Volumes/Ancillary/RAWAUXILIARY/CODEM30",
        "datafile": "COPDEM30_mosaic"
      },
      "srcpath": {
        "volume": "Ancillary",
        "hdr": "tif"
      },
      "dstpath": {
        "volume": "Ancillary",
        "hdr": "vrt"
      },
      "dstcomp": [
        {
          "copdem30": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "copdem30",
            "prefix": "dem",
            "suffix": "v01"
          }
        }
      ]
    }
  ]
}
```
