---
layout: article
title: 0160_OrganizeAncillary_CopDEM-90m.json
categories: projects
excerpt: \# Import the CopDEM 90 m virtual data to the Framework
tags:: 
    - 0160_OrganizeAncillary_CopDEM-90m.json
date: 2021-12-19
modified: 2021-12-19
comments: true
share: true
---

# 0160 OrganizeAncillary CopDEM 90m.json (projects)

### \# Import the CopDEM 90 m virtual data to the Framework

The json command file <span class='file'>0160_OrganizeAncillary_CopDEM-90m.json</span> is part of karttur's GeoImagine project <span class='project'>projects</span>. Calling the json file will execute the following commands of the GeoImagine Framework.

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
        "volume": "Ancillary",
        "hdr": "vrt"
      },
      "dstpath": {
        "volume": "Ancillary",
        "hdr": "vrt"
      },
      "srcraw": [
        {
          "copdem90": {
            "datadir": "/Volumes/Ancillary/ancillary/ESA/region/dem/global/0",
            "datafile": "dem90_copernicusdem_global_0_v01-full",
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
            "suffix": "v01-90m",
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
