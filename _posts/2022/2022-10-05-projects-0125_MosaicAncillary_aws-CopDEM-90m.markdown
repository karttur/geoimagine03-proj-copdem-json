---
layout: article
title: 0125_MosaicAncillary_aws-CopDEM-90m.json
categories: copdem90aws
excerpt:  Mosaic the AWS CopDEM 90m raw tiles
tags:: 
    - 0125_MosaicAncillary_aws-CopDEM-90m
date: 2022-10-05
modified: 2022-10-05
comments: true
share: true
---

# 0125 MosaicAncillary aws CopDEM 90m (projects)

##  Mosaic the AWS CopDEM 90m raw tiles

The json command file <span class='file'>0125_MosaicAncillary_aws-CopDEM-90m.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

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
        "getlist": "aws_tile_list",
        "srcdir": "DOWNLOADS/CopDEM90_AWS/tileList.txt"
      },
      "srcpath": {
        "volume": "GeoImg2021",
        "hdr": "tif"
      },
      "dstpath": {
        "volume": "GeoImg2021",
        "hdr": "vrt"
      },
      "dstcomp": [
        {
          "copdem90": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "copdem90",
            "prefix": "dem90",
            "suffix": "v01-aws"
          }
        }
      ]
    }
  ]
}
```
