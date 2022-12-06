---
layout: article
title: 0122_BBoxTiledRawData_gs-CopDEM-90m.json
categories: copdem90gs
excerpt:  Create polygons for all the downloaded gisco-services CopDEM tiles (optional)
tags:: 
    - 0122_BBoxTiledRawData_gs-CopDEM-90m
date: 2022-10-05
modified: 2022-10-05
comments: true
share: true
---

# 0122 BBoxTiledRawData gs CopDEM 90m (projects)

##  Create polygons for all the downloaded gisco-services CopDEM tiles (optional)

The json command file <span class='file'>0122_BBoxTiledRawData_gs-CopDEM-90m.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

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
      "processid": "BBoxTiledRawData",
      "dsversion": "1.3",
      "parameters": {
        "getlist": "csvfile-getpath1",
        "srcdir": "DOWNLOADS/CopernicusDem90/DEM/CopDEM90_tilelist.csv",
        "dstdir": "DOWNLOADS/CopernicusDem90/DEM"
      },
      "srcpath": {
        "volume": "GeoImg2021",
        "hdr": "tif"
      },
      "dstpath": {
        "volume": "GeoImg2021",
        "hdr": "shp"
      }
    }
  ]
}
```
