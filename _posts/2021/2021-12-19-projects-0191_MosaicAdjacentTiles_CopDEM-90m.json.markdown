---
layout: article
title: 0191_MosaicAdjacentTiles_CopDEM-90m.json
categories: projects
excerpt: \# Create CopDEM 90 m virtual overlap mosaics for each filled/flattened tile
tags:: 
    - 0191_MosaicAdjacentTiles_CopDEM-90m.json
date: 2021-12-19
modified: 2021-12-19
comments: true
share: true
---

# 0191 MosaicAdjacentTiles CopDEM 90m.json (projects)

### \# Create CopDEM 90 m virtual overlap mosaics for each filled/flattened tile

The json command file <span class='file'>0191_MosaicAdjacentTiles_CopDEM-90m.json</span> is part of karttur's GeoImagine project <span class='project'>projects</span>. Calling the json file will execute the following commands of the GeoImagine Framework.

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
