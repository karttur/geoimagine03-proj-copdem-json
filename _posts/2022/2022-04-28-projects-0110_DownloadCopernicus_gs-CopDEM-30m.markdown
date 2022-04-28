---
layout: article
title: 0110_DownloadCopernicus_gs-CopDEM-30m.json
categories: copdem30gs
excerpt:  Download online products for CopDEM 30 m version
tags:: 
    - 0110_DownloadCopernicus_gs-CopDEM-30m
date: 2022-04-28
modified: 2022-04-28
comments: true
share: true
---

# 0110 DownloadCopernicus gs CopDEM 30m (projects)

##  Download online products for CopDEM 30 m version

The json command file <span class='file'>0110_DownloadCopernicus_gs-CopDEM-30m.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

```
{
  "userproject": {
    "userid": "karttur",
    "projectid": "karttur",
    "tractid": "karttur",
    "siteid": "*",
    "plotid": "*",
    "system": "system"
  },
  "period": {
    "timestep": "static"
  },
  "process": [
    {
      "processid": "DownloadCopernicus",
      "dsversion": "1.3",
      "parameters": {
        "remoteuser": "Gumbricht",
        "product": "CopernicusDem90",
        "version": "",
        "serverurl": "https://gisco-services.ec.europa.eu"
      },
      "dstpath": {
        "volume": "GeoImg2021"
      }
    }
  ]
}
```
