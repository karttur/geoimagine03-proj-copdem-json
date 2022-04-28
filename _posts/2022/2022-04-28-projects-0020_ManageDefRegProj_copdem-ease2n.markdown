---
layout: article
title: 0020_ManageDefRegProj_copdem-ease2n.json
categories: common
excerpt:  Create the project environment for the CopDEM processing in the projection system ease2n
tags:: 
    - 0020_ManageDefRegProj_copdem-ease2n
date: 2022-04-28
modified: 2022-04-28
comments: true
share: true
---

# 0020 ManageDefRegProj copdem ease2n (projects)

##  Create the project environment for the CopDEM processing in the projection system ease2n

The json command file <span class='file'>0020_ManageDefRegProj_copdem-ease2n.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

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
      "processid": "ManageDefRegProj",
      "overwrite": false,
      "parameters": {
        "defaultregion": "northlandease2n",
        "tractid": "karttur-northlandease2n",
        "tractname": "karttur northlandease2n",
        "projid": "karttur-northlandease2n",
        "projname": "karttur northlandease2n",
        "tracttitle": "Karttur northlandease2n",
        "tractlabel": "Karttur northlandease2n",
        "projtitle": "Karttur northlandease2n",
        "projlabel": "Karttur northlandease2n"
      }
    }
  ]
}
```
