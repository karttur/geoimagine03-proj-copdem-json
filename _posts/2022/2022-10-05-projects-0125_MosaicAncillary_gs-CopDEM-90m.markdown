---
layout: article
title: 0125_MosaicAncillary_gs-CopDEM-90m.json
categories: copdem90gs
excerpt:  Mosaic the gisco-services CopDEM 90m raw tiles
tags:: 
    - 0125_MosaicAncillary_gs-CopDEM-90m
date: 2022-10-05
modified: 2022-10-05
comments: true
share: true
---

# 0125 MosaicAncillary gs CopDEM 90m (projects)

##  Mosaic the gisco-services CopDEM 90m raw tiles

The json command file <span class='file'>0125_MosaicAncillary_gs-CopDEM-90m.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

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
        "datadir": "DOWNLOADS/CopernicusDem90/DEM"
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
          "copernicusdem90": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "copdem90",
            "prefix": "dem90",
            "suffix": "v01"
          }
        }
      ]
    }
  ]
}
```
