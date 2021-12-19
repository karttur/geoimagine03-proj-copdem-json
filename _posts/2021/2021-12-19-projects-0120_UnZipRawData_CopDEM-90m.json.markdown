---
layout: article
title: 0120_UnZipRawData_CopDEM-90m.json
categories: projects
excerpt: \# Explode (UnZip) donwloaded CopDem 90m products
tags:: 
    - 0120_UnZipRawData_CopDEM-90m.json
date: 2021-12-19
modified: 2021-12-19
comments: true
share: true
---

# 0120 UnZipRawData CopDEM 90m.json (projects)

### \# Explode (UnZip) donwloaded CopDem 90m products

The json command file <span class='file'>0120_UnZipRawData_CopDEM-90m.json</span> is part of karttur's GeoImagine project <span class='project'>projects</span>. Calling the json file will execute the following commands of the GeoImagine Framework.

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
      "processid": "UnZipRawData",
      "dsversion": "1.3",
      "parameters": {
        "path": "/Volumes/Ancillary/DOWNLOADS/CopernicusDem90/CopernicusDem90-0.csv",
        "rootdir": "RAWAUXILIARY/CopernicusDem90",
        "srcsubdir": "",
        "dstsubdir": "DEM",
        "getlist": "csvfile-getpath1",
        "pattern": "DEM",
        "zipreplace": ".tif",
        "minlon": -180,
        "maxlon": 180,
        "minlat": -90,
        "maxlat": 90
      },
      "srcpath": {
        "volume": "Ancillary"
      },
      "dstpath": {
        "volume": "Ancillary"
      }
    }
  ]
}
```
