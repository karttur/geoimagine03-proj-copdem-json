---
layout: article
title: 0192_MosaicAdjacentTiles_CopDEM-90m.json
categories: projects
excerpt: \# Create virtual overlaps of the twice filled CopDEM 90m
tags:: 
    - 0192_MosaicAdjacentTiles_CopDEM-90m.json
date: 2021-12-19
modified: 2021-12-19
comments: true
share: true
---

# 0192 MosaicAdjacentTiles CopDEM 90m.json (projects)

### \# Create virtual overlaps of the twice filled CopDEM 90m

The json command file <span class='file'>0192_MosaicAdjacentTiles_CopDEM-90m.json</span> is part of karttur's GeoImagine project <span class='project'>projects</span>. Calling the json file will execute the following commands of the GeoImagine Framework.

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
