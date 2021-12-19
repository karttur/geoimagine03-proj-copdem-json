---
layout: article
title: 0125_MosaicAncillary_CopDEM-90m.json
categories: projects
excerpt: \# Mosaic the CopDEM 90m data
tags:: 
    - 0125_MosaicAncillary_CopDEM-90m.json
date: 2021-12-19
modified: 2021-12-19
comments: true
share: true
---

# 0125 MosaicAncillary CopDEM 90m.json (projects)

### \# Mosaic the CopDEM 90m data

The json command file <span class='file'>0125_MosaicAncillary_CopDEM-90m.json</span> is part of karttur's GeoImagine project <span class='project'>projects</span>. Calling the json file will execute the following commands of the GeoImagine Framework.

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
        "datadir": "RAWAUXILIARY/CopernicusDem90/DEM",
        "datafile": "CopernicusDem90_mosaic"
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
          "copernicusdem90": {
            "source": "ESA",
            "product": "copernicusdem",
            "content": "dem",
            "layerid": "copernicusdem90",
            "prefix": "dem90",
            "suffix": "v01"
          }
        }
      ]
    }
  ]
}
```
