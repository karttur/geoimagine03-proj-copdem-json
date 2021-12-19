---
layout: article
title: 0180_TileAncillaryRegion_CopDem-30m.json
categories: projects
excerpt: \# Tile the virtual CopDEM 30 m mosaic to tif tiles
tags:: 
    - 0180_TileAncillaryRegion_CopDem-30m.json
date: 2021-12-19
modified: 2021-12-19
comments: true
share: true
---

# 0180 TileAncillaryRegion CopDem 30m.json (projects)

### \# Tile the virtual CopDEM 30 m mosaic to tif tiles

The json command file <span class='file'>0180_TileAncillaryRegion_CopDem-30m.json</span> is part of karttur's GeoImagine project <span class='project'>projects</span>. Calling the json file will execute the following commands of the GeoImagine Framework.

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
        "defregid": "global",
        "tr_xres": 30,
        "tr_yres": 30,
        "resample": "bilinear",
        "asscript": true
      },
      "srcpath": {
        "volume": "Ancillary",
        "hdr": "vrt"
      },
      "dstpath": {
        "volume": "Ancillary",
        "hdr": "tif"
      },
      "srccomp": [
        {
          "copdem30": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "copdem",
            "prefix": "dem",
            "suffix": "v01-30m",
            "cellnull": -32767
          }
        }
      ],
      "dstcopy": [
        {
          "copdem30": {
            "srccomp": "dem_copdem"
          }
        }
      ]
    }
  ]
}
```
