---
layout: article
title: 0122_BBoxTiledRawData_aws-CopDEM-90m.json
categories: copdem90aws
excerpt:  Create polygons for all the downloaded AWS CopDEM tiles (optional)
tags:: 
    - 0122_BBoxTiledRawData_aws-CopDEM-90m
date: 2022-04-28
modified: 2022-04-28
comments: true
share: true
---

# 0122 BBoxTiledRawData aws CopDEM 90m (projects)

##  Create polygons for all the downloaded AWS CopDEM tiles (optional)

The json command file <span class='file'>0122_BBoxTiledRawData_aws-CopDEM-90m.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

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
        "getlist": "aws_tile_list",
        "srcdir": "DOWNLOADS/CopDEM90_AWS/tileList.txt",
        "dstdir": "DOWNLOADS/CopDEM90_AWS/tiles2"
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
