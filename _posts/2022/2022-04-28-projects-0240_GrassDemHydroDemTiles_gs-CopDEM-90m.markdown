---
layout: article
title: 0240_GrassDemHydroDemTiles_gs-CopDEM-90m.json
categories: copdem90gs
excerpt:  Fill larger pits in streams of CopDEM 90 m with r.hydrodem
tags:: 
    - 0240_GrassDemHydroDemTiles_gs-CopDEM-90m
date: 2022-04-28
modified: 2022-04-28
comments: true
share: true
---

# 0240 GrassDemHydroDemTiles gs CopDEM 90m (projects)

##  Fill larger pits in streams of CopDEM 90 m with r.hydrodem

The json command file <span class='file'>0240_GrassDemHydroDemTiles_gs-CopDEM-90m.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

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
      "processid": "GrassDemHydroDemTiles",
      "version": "1.3",
      "overwrite": true,
      "parameters": {
        "asscript": true,
        "mosaic": true,
        "superimpose": true,
        "size":10,
        "mod":5,
        "memory":3000,
        "query": "u_maximum >= 500"
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
            "suffix": "v01-pfpf-hydrdem4+4-90m"
          }
        }
      ]
    }
  ]
}
```
