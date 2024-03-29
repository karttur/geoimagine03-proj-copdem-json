---
layout: article
title: 0120_UnZipRawData_gs-CopDEM-30m.json
categories: copdem30gs
excerpt:  Explode (UnZip) downloaded CopDem 30m products
tags:: 
    - 0120_UnZipRawData_gs-CopDEM-30m
date: 2022-10-05
modified: 2022-10-05
comments: true
share: true
---

# 0120 UnZipRawData gs CopDEM 30m (projects)

##  Explode (UnZip) downloaded CopDem 30m products

The json command file <span class='file'>0120_UnZipRawData_gs-CopDEM-30m.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

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
        "srcdir": "DOWNLOADS/CopernicusDem90/CopernicusDem90_rawtiles.csv",
        "dstdir": "DOWNLOADS/CopernicusDem90/DEM",
        "getlist": "csvfile-getpath1",
        "pattern": "DEM",
        "zipreplace": ".tif",
        "minlon": -180,
        "maxlon": 180,
        "minlat": -90,
        "maxlat": 90
      },
      "dstpath": {
        "volume": "GeoImg2021",
        "hdr": "tif"
      }
    }
  ]
}
```
