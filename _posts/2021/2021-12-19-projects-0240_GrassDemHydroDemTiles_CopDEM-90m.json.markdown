---
layout: article
title: 0240_GrassDemHydroDemTiles_CopDEM-90m.json
categories: projects
excerpt: \# Fill larger pits in streams of CopDEM 90 m with r.hydrodem
tags:: 
    - 0240_GrassDemHydroDemTiles_CopDEM-90m.json
date: 2021-12-19
modified: 2021-12-19
comments: true
share: true
---

# 0240 GrassDemHydroDemTiles CopDEM 90m.json (projects)

### \# Fill larger pits in streams of CopDEM 90 m with r.hydrodem

The json command file <span class='file'>0240_GrassDemHydroDemTiles_CopDEM-90m.json</span> is part of karttur's GeoImagine project <span class='project'>projects</span>. Calling the json file will execute the following commands of the GeoImagine Framework.

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
