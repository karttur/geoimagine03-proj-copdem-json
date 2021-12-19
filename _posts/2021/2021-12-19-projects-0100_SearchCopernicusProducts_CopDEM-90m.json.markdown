---
layout: article
title: 0100_SearchCopernicusProducts_CopDEM-90m.json
categories: projects
excerpt: \# Search online products for CopDEM 90 m version
tags:: 
    - 0100_SearchCopernicusProducts_CopDEM-90m.json
date: 2021-12-19
modified: 2021-12-19
comments: true
share: true
---

# 0100 SearchCopernicusProducts CopDEM 90m.json (projects)

### \# Search online products for CopDEM 90 m version

The json command file <span class='file'>0100_SearchCopernicusProducts_CopDEM-90m.json</span> is part of karttur's GeoImagine project <span class='project'>projects</span>. Calling the json file will execute the following commands of the GeoImagine Framework.

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
      "srcpath": {
        "volume": "GeoImg2021"
      },
      "dstpath": {
        "volume": "GeoImg2021"
      }
    }
  ]
}
```
