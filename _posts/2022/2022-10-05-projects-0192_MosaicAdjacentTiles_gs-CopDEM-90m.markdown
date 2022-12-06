---
layout: article
title: 0192_MosaicAdjacentTiles_gs-CopDEM-90m.json
categories: copdem90gs
excerpt:  Create virtual overlaps of the twice filled CopDEM 90m
tags:: 
    - 0192_MosaicAdjacentTiles_gs-CopDEM-90m
date: 2022-10-05
modified: 2022-10-05
comments: true
share: true
---

# 0192 MosaicAdjacentTiles gs CopDEM 90m (projects)

##  Create virtual overlaps of the twice filled CopDEM 90m

The json command file <span class='file'>0192_MosaicAdjacentTiles_gs-CopDEM-90m.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

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
      "processid": "MosaicAdjacentTiles",
      "version": "1.3",
      "overwrite": true,
      "parameters": {
        "tr_xres": 90,
        "tr_yres": 90,
        "overlap": 501,
        "resample": "near",
        "asscript": true
      },
      "srcpath": {
        "volume": "Ancillary",
        "hdr": "tif"
      },
      "dstpath": {
        "volume": "Ancillary",
        "hdr": "vrt"
      },
      "srccomp": [
        {
          "copdem90": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "copdem",
            "prefix": "dem",
            "suffix": "v01-pfpf-hydrdem4+4-90m",
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
