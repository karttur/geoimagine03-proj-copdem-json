---
layout: article
title: 0100_SearchCopernicusProducts_gs-CopDEM-90m.json
categories: copdem90gs
excerpt:  Search gisco-services online products for CopDEM 90 m version
tags:: 
    - 0100_SearchCopernicusProducts_gs-CopDEM-90m
date: 2022-10-05
modified: 2022-10-05
comments: true
share: true
---

# 0100 SearchCopernicusProducts gs CopDEM 90m (projects)

##  Search gisco-services online products for CopDEM 90 m version

The json command file <span class='file'>0100_SearchCopernicusProducts_gs-CopDEM-90m.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

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
      "processid": "SearchCopernicusProducts",
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
