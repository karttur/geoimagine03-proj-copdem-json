---
layout: article
title: 0230_GrassDemFillDirTiles_gs-CopDEM_90m.json
categories: copdem90gs
excerpt:  Fill single pits and peaks (adjacent to streams)
tags:: 
    - 0230_GrassDemFillDirTiles_gs-CopDEM_90m
date: 2022-10-05
modified: 2022-10-05
comments: true
share: true
---

# 0230 GrassDemFillDirTiles gs CopDEM 90m (projects)

##  Fill single pits and peaks (adjacent to streams)

The json command file <span class='file'>0230_GrassDemFillDirTiles_gs-CopDEM_90m.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

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
