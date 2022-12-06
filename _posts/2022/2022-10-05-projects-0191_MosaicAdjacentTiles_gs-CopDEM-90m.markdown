---
layout: article
title: 0191_MosaicAdjacentTiles_gs-CopDEM-90m.json
categories: copdem90gs
excerpt:  Create CopDEM 90 m virtual overlap mosaics for each filled/flattened tile
tags:: 
    - 0191_MosaicAdjacentTiles_gs-CopDEM-90m
date: 2022-10-05
modified: 2022-10-05
comments: true
share: true
---

# 0191 MosaicAdjacentTiles gs CopDEM 90m (projects)

##  Create CopDEM 90 m virtual overlap mosaics for each filled/flattened tile

The json command file <span class='file'>0191_MosaicAdjacentTiles_gs-CopDEM-90m.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

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
      "overwrite": false,
      "parameters": {
        "tr_xres": 90,
        "tr_yres": 90,
        "resample": "near",
        "asscript": true
      },
      "srcpath": {
        "volume": "Arctic2021",
        "hdr": "tif"
      },
      "dstpath": {
        "volume": "Arctic2021",
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
            "suffix": "v01-pfpf-90m",
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
