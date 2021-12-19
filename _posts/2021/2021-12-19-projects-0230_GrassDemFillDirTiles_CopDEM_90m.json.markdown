---
layout: article
title: 0230_GrassDemFillDirTiles_CopDEM_90m.json
categories: projects
excerpt: \# Fill single pits and peaks (adjacent to streams)
tags:: 
    - 0230_GrassDemFillDirTiles_CopDEM_90m.json
date: 2021-12-19
modified: 2021-12-19
comments: true
share: true
---

# 0230 GrassDemFillDirTiles CopDEM 90m.json (projects)

### \# Fill single pits and peaks (adjacent to streams)

The json command file <span class='file'>0230_GrassDemFillDirTiles_CopDEM_90m.json</span> is part of karttur's GeoImagine project <span class='project'>projects</span>. Calling the json file will execute the following commands of the GeoImagine Framework.

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
      "processid": "GrassDemFillDirTiles",
      "version": "1.3",
      "overwrite": false,
      "parameters": {
        "asscript": true,
        "superimpose": false,
        "pitsize": 1,
        "pitquery": "",
        "peaks": true,
        "peakquery": "nbupmax >= 500 AND nbupq3 >= 250",
        "mosaic": true
      },
      "srcpath": {
        "volume": "Ancillary",
        "hdr": "tif"
      },
      "dstpath": {
        "volume": "Ancillary",
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
            "suffix": "v01-90m"
          }
        }
      ],
      "dstcopy": [
        {
          "copdem90": {
            "source": "copy",
            "product": "copy",
            "content": "copy",
            "layerid": "copy",
            "prefix": "copy",
            "suffix": "v01-pfpf-90m"
          }
        }
      ]
    },
    {
      "processid": "GrassDemHydroDemTiles",
      "version": "1.3",
      "overwrite": true,
      "parameters": {
        "asscript": true,
        "superimpose": true,
        "mosaic": true,
        "size": 4,
        "mod": 8,
        "query": "updrain >= 500 or area_cells = 1"
      },
      "srcpath": {
        "volume": "Ancillary",
        "hdr": "tif"
      },
      "dstpath": {
        "volume": "Ancillary",
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
            "suffix": "v01-pfpf-90m"
          }
        }
      ],
      "dstcopy": [
        {
          "copdem90": {
            "source": "copy",
            "product": "copy",
            "content": "copy",
            "layerid": "copy",
            "prefix": "copy",
            "suffix": "v01-pfpfhd-90m"
          }
        }
      ]
    }
  ]
}
```
