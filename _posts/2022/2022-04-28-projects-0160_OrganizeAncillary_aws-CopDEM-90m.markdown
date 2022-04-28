---
layout: article
title: 0160_OrganizeAncillary_aws-CopDEM-90m.json
categories: copdem90aws
excerpt:  Import the virtual data to the Framework
tags:: 
    - 0160_OrganizeAncillary_aws-CopDEM-90m
date: 2022-04-28
modified: 2022-04-28
comments: true
share: true
---

# 0160 OrganizeAncillary aws CopDEM 90m (projects)

##  Import the virtual data to the Framework

The json command file <span class='file'>0160_OrganizeAncillary_aws-CopDEM-90m.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

```
{
  "userproject": {
    "userid": "karttur",
    "projectid": "karttur",
    "tractid": "karttur",
    "siteid": "*",
    "plotid": "*",
    "system": "ancillary"
  },
  "period": {
    "timestep": "static"
  },
  "process": [
    {
      "processid": "OrganizeAncillary",
      "overwrite": false,
      "parameters": {
        "importcode": "vrt",
        "epsg": "4326",
        "orgid": "ESA",
        "dsname": "coperdicusdem90",
        "dsversion": "1.0",
        "accessdate": "20210320",
        "regionid": "global",
        "regioncat": "global",
        "dataurl": "https://registry.opendata.aws/copernicus-dem/",
        "metaurl": "https://docs.sentinel-hub.com/api/latest/data/dem/",
        "title": "Copernicus DEM global 90 m",
        "label": "Copernicus DEM global 90 m"
      },
      "srcpath": {
        "volume": "GeoImg2021",
        "hdr": "vrt"
      },
      "dstpath": {
        "volume": "GeoImg2021",
        "hdr": "vrt"
      },
      "srcraw": [
        {
          "copdem90": {
            "datadir": "ancillary/ESA/region/dem/global/0",
            "datafile": "dem90_copdem_global_0_v01-aws",
            "datalayer": "DEM",
            "title": "Copernicus DEM global 90 m",
            "label": "Copernicus DEM global 90 m"
          }
        }
      ],
      "dstcomp": [
        {
          "copdem90": {
            "source": "ESA",
            "product": "copdem",
            "content": "dem",
            "layerid": "copdem",
            "prefix": "dem",
            "suffix": "v01-aws-90m",
            "scalefac": 1,
            "offsetadd": 0,
            "dataunit": "masl",
            "celltype": "Float32",
            "cellnull": -32767,
            "measure": "R",
            "masked": "N"
          }
        }
      ]
    }
  ]
}
```
