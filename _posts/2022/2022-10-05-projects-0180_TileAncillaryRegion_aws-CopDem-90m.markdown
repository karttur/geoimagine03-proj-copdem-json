---
layout: article
title: 0180_TileAncillaryRegion_aws-CopDem-90m.json
categories: copdem90aws
excerpt:  Tile the virtual mosaic to tif tiles
tags:: 
    - 0180_TileAncillaryRegion_aws-CopDem-90m
date: 2022-10-05
modified: 2022-10-05
comments: true
share: true
---

# 0180 TileAncillaryRegion aws CopDem 90m (projects)

##  Tile the virtual mosaic to tif tiles

The json command file <span class='file'>0180_TileAncillaryRegion_aws-CopDem-90m.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

```
{
  "userproject": {
    "userid": "karttur",
    "projectid": "karttur-northlandease2n",
    "tractid": "karttur-northlandease2n",
    "siteid": "*",
    "plotid": "*",
    "system": "ease2n"
  },
  "period": {
    "timestep": "static"
  },
  "process": [
    {
      "processid": "TileAncillaryRegion",
      "version": "1.3",
      "overwrite": false,
      "parameters": {
        "src_defregid": "global",
        "tr_xres": 90,
        "tr_yres": 90,
        "resample": "bilinear",
        "asscript": true
      },
      "srcpath": {
        "volume": "GeoImg2021",
        "hdr": "vrt"
      },
      "dstpath": {
        "volume": "GeoImg2021",
        "hdr": "tif"
      },
      "srccomp": [
        {
          "copdem90": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "copdem",
            "prefix": "dem",
            "suffix": "v01-aws-90m",
            "cellnull": -32767
          }
        }
      ],
      "dstcopy": [
        {
          "copdem90": {
            "srccomp": "dem_copdem"
          }
        }
      ]
    }
  ]
}
```
