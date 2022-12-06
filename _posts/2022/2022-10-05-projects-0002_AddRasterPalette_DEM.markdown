---
layout: article
title: 0002_AddRasterPalette_DEM_v090.json
categories: common
excerpt:  Add raster palette for byte range DEM data
tags:: 
    - 0002_AddRasterPalette_DEM
date: 2022-10-05
modified: 2022-10-05
comments: true
share: true
---

# 0002 AddRasterPalette DEM (projects)

##  Add raster palette for byte range DEM data

The json command file <span class='file'>0002_AddRasterPalette_DEM_v090.json</span> is part of Karttur's GeoImagine project [<span class='project'>CopDEM</span>](https://karttur.github.io/geoimagine03-proj-copdem/index.html). For details on the commands see the blog on [Framework Processes](https://karttur.github.io/geoimagine03-docs-procpack/).

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
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "dem_dark_auto",
        "compid": "dem_dark_auto",
        "setcolor": {
          "0": {
            "red": "54",
            "green": "121",
            "blue": "36",
            "alpha": "0",
            "label": "auto",
            "hint": "auto"
          },
          "125": {
            "red": "247",
            "green": "248",
            "blue": "80",
            "alpha": "0",
            "label": "auto",
            "hint": "auto"
          },
          "250": {
            "red": "121",
            "green": "24",
            "blue": "21",
            "alpha": "0",
            "label": "auto",
            "hint": "auto"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "landformTPI",
        "compid": "dem_landform-TPI",
        "setcolor": {
          "5": {
            "red": "30",
            "green": "0",
            "blue": "170",
            "alpha": "0",
            "label": "Canyon or valley",
            "hint": "NA"
          },
          "12": {
            "red": "30",
            "green": "0",
            "blue": "170",
            "alpha": "0",
            "label": "Canyon or valley",
            "hint": "Canyon or valley"
          },
          "13": {
            "red": "10",
            "green": "160",
            "blue": "10",
            "alpha": "0",
            "label": "midslope/shallow valley, hollow",
            "hint": "NA"
          },
          "22": {
            "red": "10",
            "green": "160",
            "blue": "10",
            "alpha": "0",
            "label": "midslope/shallow valley, hollow",
            "hint": "midslope/shallow valley, hollow"
          },
          "23": {
            "red": "25",
            "green": "155",
            "blue": "234",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "NA"
          },
          "32": {
            "red": "25",
            "green": "155",
            "blue": "234",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "33": {
            "red": "0",
            "green": "128",
            "blue": "128",
            "alpha": "0",
            "label": "U-shaped valley or footslope",
            "hint": "NA"
          },
          "42": {
            "red": "0",
            "green": "128",
            "blue": "128",
            "alpha": "0",
            "label": "U-shaped valley or footslope",
            "hint": "U-shaped valley or footslope"
          },
          "43": {
            "red": "220",
            "green": "235",
            "blue": "240",
            "alpha": "0",
            "label": "plain",
            "hint": "NA"
          },
          "52": {
            "red": "220",
            "green": "235",
            "blue": "240",
            "alpha": "0",
            "label": "plain",
            "hint": "plain or flat"
          },
          "53": {
            "red": "230",
            "green": "230",
            "blue": "120",
            "alpha": "0",
            "label": "open slope",
            "hint": "NA"
          },
          "62": {
            "red": "230",
            "green": "230",
            "blue": "120",
            "alpha": "0",
            "label": "open slope",
            "hint": "open slope"
          },
          "63": {
            "red": "235",
            "green": "205",
            "blue": "15",
            "alpha": "0",
            "label": "upper slope",
            "hint": "NA"
          },
          "72": {
            "red": "235",
            "green": "205",
            "blue": "15",
            "alpha": "0",
            "label": "upper slope",
            "hint": "mesa, upper slope, shoulder, ridge"
          },
          "73": {
            "red": "255",
            "green": "128",
            "blue": "10",
            "alpha": "0",
            "label": "local ridge",
            "hint": "NA"
          },
          "82": {
            "red": "255",
            "green": "128",
            "blue": "10",
            "alpha": "0",
            "label": "local ridge",
            "hint": "lodal ridge"
          },
          "83": {
            "red": "224",
            "green": "80",
            "blue": "80",
            "alpha": "0",
            "label": "midslope ridge or spur",
            "hint": "NA"
          },
          "92": {
            "red": "224",
            "green": "80",
            "blue": "80",
            "alpha": "0",
            "label": "midslope ridge or spur",
            "hint": "midslope ridge or spur"
          },
          "93": {
            "red": "180",
            "green": "20",
            "blue": "10",
            "alpha": "0",
            "label": "peak",
            "hint": "NA"
          },
          "102": {
            "red": "180",
            "green": "20",
            "blue": "10",
            "alpha": "0",
            "label": "peak",
            "hint": "peak or summit"
          },
          "107": {
            "red": "180",
            "green": "20",
            "blue": "10",
            "alpha": "0",
            "label": "peak",
            "hint": "NA"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "255",
            "label": "255",
            "hint": "no data"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "landformTPIdouble",
        "compid": "landform-TPIx",
        "setcolor": {
          "11": {
            "red": "0",
            "green": "0",
            "blue": "200",
            "alpha": "0",
            "label": "Canyon or valley",
            "hint": "Canyon or valley"
          },
          "12": {
            "red": "55",
            "green": "0",
            "blue": "150",
            "alpha": "0",
            "label": "Canyon or valley",
            "hint": "Canyon or valley"
          },
          "21": {
            "red": "0",
            "green": "200",
            "blue": "0",
            "alpha": "0",
            "label": "shallow valley",
            "hint": "shallow valley or hollow"
          },
          "22": {
            "red": "0",
            "green": "180",
            "blue": "135",
            "alpha": "0",
            "label": "midslope drainage",
            "hint": " midslope drainage or shallow valley or hollow"
          },
          "31": {
            "red": "50",
            "green": "50",
            "blue": "200",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "32": {
            "red": "25",
            "green": "25",
            "blue": "225",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "41": {
            "red": "0",
            "green": "155",
            "blue": "244",
            "alpha": "0",
            "label": "U-shaped valley",
            "hint": "U-shaped valley or footslope"
          },
          "42": {
            "red": "0",
            "green": "100",
            "blue": "200",
            "alpha": "0",
            "label": "Footslope",
            "hint": "U-shaped valley or footslope"
          },
          "50": {
            "red": "220",
            "green": "220",
            "blue": "220",
            "alpha": "0",
            "label": "plain",
            "hint": "plain or flat"
          },
          "60": {
            "red": "251",
            "green": "255",
            "blue": "0",
            "alpha": "0",
            "label": "open slope",
            "hint": "open slope"
          },
          "71": {
            "red": "255",
            "green": "56",
            "blue": "0",
            "alpha": "0",
            "label": "upper slope",
            "hint": "upper slope, shoulder, ridge"
          },
          "72": {
            "red": "130",
            "green": "130",
            "blue": "0",
            "alpha": "0",
            "label": "mesa",
            "hint": "mesa, upper slope, shoulder, ridge"
          },
          "81": {
            "red": "255",
            "green": "213",
            "blue": "112",
            "alpha": "0",
            "label": "local ridge",
            "hint": "lodal ridge (midslope)"
          },
          "82": {
            "red": "255",
            "green": "213",
            "blue": "112",
            "alpha": "0",
            "label": "local ridge",
            "hint": "local ridge (in plain)"
          },
          "91": {
            "red": "254",
            "green": "214",
            "blue": "0",
            "alpha": "0",
            "label": "midslope ridge or spur",
            "hint": "midslope ridge or spur"
          },
          "92": {
            "red": "254",
            "green": "214",
            "blue": "0",
            "alpha": "0",
            "label": "midslope ridge or spur",
            "hint": "midslope ridge or spur"
          },
          "101": {
            "red": "140",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "peak",
            "hint": "peak or summit"
          },
          "102": {
            "red": "100",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "peak",
            "hint": "peak or summit"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "255",
            "label": "255",
            "hint": "no data"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "slope",
        "compid": "dem_slope",
        "setcolor": {
          "0": {
            "red": "0",
            "green": "92",
            "blue": "128",
            "alpha": "0",
            "label": "0",
            "hint": "slope = 0 (flat)"
          },
          "4": {
            "red": "0",
            "green": "128",
            "blue": "64",
            "alpha": "0",
            "label": "1.0",
            "hint": "NA"
          },
          "40": {
            "red": "220",
            "green": "240",
            "blue": "16",
            "alpha": "0",
            "label": "10",
            "hint": "slope = 10"
          },
          "80": {
            "red": "255",
            "green": "146",
            "blue": "18",
            "alpha": "0",
            "label": "30",
            "hint": "slope = 30"
          },
          "160": {
            "red": "192",
            "green": "46",
            "blue": "0",
            "alpha": "0",
            "label": "50",
            "hint": "slope = 50"
          },
          "250": {
            "red": "128",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "> 60",
            "hint": "slope > 60"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "slope2",
        "compid": "dem_slope2",
        "setcolor": {
          "0": {
            "red": "143",
            "green": "152",
            "blue": "18",
            "alpha": "0",
            "label": "0",
            "hint": "slope = 0 (flat)"
          },
          "4": {
            "red": "150",
            "green": "160",
            "blue": "33",
            "alpha": "0",
            "label": "1.0",
            "hint": "NA"
          },
          "40": {
            "red": "225",
            "green": "240",
            "blue": "51",
            "alpha": "0",
            "label": "10",
            "hint": "slope = 10"
          },
          "80": {
            "red": "255",
            "green": "200",
            "blue": "10",
            "alpha": "0",
            "label": "20",
            "hint": "slope = 20"
          },
          "120": {
            "red": "250",
            "green": "160",
            "blue": "40",
            "alpha": "0",
            "label": "30",
            "hint": "slope = 30"
          },
          "160": {
            "red": "245",
            "green": "100",
            "blue": "20",
            "alpha": "0",
            "label": "40",
            "hint": "slope = 40"
          },
          "200": {
            "red": "205",
            "green": "70",
            "blue": "120",
            "alpha": "0",
            "label": "50",
            "hint": "slope = 50"
          },
          "250": {
            "red": "179",
            "green": "107",
            "blue": "209",
            "alpha": "0",
            "label": "> 60",
            "hint": "slope > 60"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "slope3",
        "compid": "dem_slope3",
        "setcolor": {
          "0": {
            "red": "135",
            "green": "160",
            "blue": "212",
            "alpha": "0",
            "label": "0",
            "hint": "slope = 0 (flat)"
          },
          "4": {
            "red": "168",
            "green": "179",
            "blue": "149",
            "alpha": "0",
            "label": "1.0",
            "hint": "NA"
          },
          "40": {
            "red": "213",
            "green": "222",
            "blue": "115",
            "alpha": "0",
            "label": "10",
            "hint": "slope = 10"
          },
          "80": {
            "red": "253",
            "green": "253",
            "blue": "155",
            "alpha": "0",
            "label": "20",
            "hint": "slope = 20"
          },
          "120": {
            "red": "239",
            "green": "184",
            "blue": "12",
            "alpha": "0",
            "label": "30",
            "hint": "slope = 30"
          },
          "160": {
            "red": "223",
            "green": "144",
            "blue": "88",
            "alpha": "0",
            "label": "40",
            "hint": "slope = 40"
          },
          "200": {
            "red": "233",
            "green": "129",
            "blue": "189",
            "alpha": "0",
            "label": "50",
            "hint": "slope = 50"
          },
          "250": {
            "red": "216",
            "green": "153",
            "blue": "243",
            "alpha": "0",
            "label": "> 60",
            "hint": "slope > 60"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "peakproximity",
        "compid": "terrain_peakproximity",
        "setcolor": {
          "0": {
            "red": "128",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "slope",
            "hint": "slopee"
          },
          "5": {
            "red": "225",
            "green": "175",
            "blue": "0",
            "alpha": "0",
            "label": "slope",
            "hint": "slope"
          },
          "50": {
            "red": "175",
            "green": "225",
            "blue": "0",
            "alpha": "0",
            "label": "slope",
            "hint": "slope"
          },
          "150": {
            "red": "0",
            "green": "125",
            "blue": "125",
            "alpha": "0",
            "label": "slope",
            "hint": "slope"
          },
          "250": {
            "red": "0",
            "green": "0",
            "blue": "128",
            "alpha": "0",
            "label": "flat",
            "hint": "flat"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "generalproximity",
        "compid": "any_proximity",
        "setcolor": {
          "0": {
            "red": "252",
            "green": "246",
            "blue": "120",
            "alpha": "0",
            "label": "0",
            "hint": "0 (no distance)"
          },
          "28": {
            "red": "127",
            "green": "207",
            "blue": "120",
            "alpha": "0",
            "label": "0.5",
            "hint": "distance = 0.5 km"
          },
          "56": {
            "red": "127",
            "green": "207",
            "blue": "220",
            "alpha": "0",
            "label": "1.0",
            "hint": "distance = 1.0 km"
          },
          "224": {
            "red": "151",
            "green": "10",
            "blue": "151",
            "alpha": "0",
            "label": "4.0",
            "hint": "distance = 4.0 km"
          },
          "249": {
            "red": "151",
            "green": "10",
            "blue": "151",
            "alpha": "0",
            "label": "4.5",
            "hint": "NA"
          },
          "250": {
            "red": "151",
            "green": "10",
            "blue": "151",
            "alpha": "0",
            "label": "> 4.5",
            "hint": "distance > 4.5 km"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "near-divide-dist",
        "compid": "terrain_near-divide-dist",
        "setcolor": {
          "0": {
            "red": "252",
            "green": "246",
            "blue": "120",
            "alpha": "0",
            "label": "0",
            "hint": "0 (no distance)"
          },
          "25": {
            "red": "127",
            "green": "207",
            "blue": "120",
            "alpha": "0",
            "label": "0.25",
            "hint": "distance = 0.25 km"
          },
          "50": {
            "red": "127",
            "green": "207",
            "blue": "220",
            "alpha": "0",
            "label": "0.5",
            "hint": "distance = 0.5 km"
          },
          "100": {
            "red": "135",
            "green": "110",
            "blue": "250",
            "alpha": "0",
            "label": "1.0",
            "hint": "distance = 1.0 km"
          },
          "200": {
            "red": "135",
            "green": "10",
            "blue": "210",
            "alpha": "0",
            "label": "2.0",
            "hint": "distance = 2.0 km"
          },
          "249": {
            "red": "160",
            "green": "10",
            "blue": "160",
            "alpha": "0",
            "label": "auto",
            "hint": "NA"
          },
          "250": {
            "red": "121",
            "green": "5",
            "blue": "121",
            "alpha": "0",
            "label": "> 2.5",
            "hint": "distance > 2.5 km"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "far-divide-dist",
        "compid": "terrain_far-divide-dist",
        "setcolor": {
          "0": {
            "red": "252",
            "green": "246",
            "blue": "120",
            "alpha": "0",
            "label": "0",
            "hint": "0 (no distance)"
          },
          "25": {
            "red": "127",
            "green": "207",
            "blue": "120",
            "alpha": "0",
            "label": "2.5",
            "hint": "distance = 2.5 km"
          },
          "50": {
            "red": "127",
            "green": "207",
            "blue": "220",
            "alpha": "0",
            "label": "5.0",
            "hint": "distance = 5.0 km"
          },
          "100": {
            "red": "135",
            "green": "110",
            "blue": "250",
            "alpha": "0",
            "label": "10",
            "hint": "distance = 10 km"
          },
          "200": {
            "red": "135",
            "green": "10",
            "blue": "210",
            "alpha": "0",
            "label": "20",
            "hint": "distance = 20 km"
          },
          "249": {
            "red": "160",
            "green": "10",
            "blue": "160",
            "alpha": "0",
            "label": "auto",
            "hint": "NA"
          },
          "250": {
            "red": "121",
            "green": "5",
            "blue": "121",
            "alpha": "0",
            "label": "> 25",
            "hint": "distance > 25 km"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "generalproximity",
        "compid": "any_proximity",
        "setcolor": {
          "0": {
            "red": "252",
            "green": "246",
            "blue": "120",
            "alpha": "0",
            "label": "auto",
            "hint": "0 (no distance)"
          },
          "28": {
            "red": "127",
            "green": "207",
            "blue": "120",
            "alpha": "0",
            "label": "auto",
            "hint": "distance = 0.5 km"
          },
          "56": {
            "red": "127",
            "green": "207",
            "blue": "220",
            "alpha": "0",
            "label": "auto",
            "hint": "distance = 1.0 km"
          },
          "224": {
            "red": "151",
            "green": "10",
            "blue": "151",
            "alpha": "0",
            "label": "auto",
            "hint": "distance = 4.0 km"
          },
          "249": {
            "red": "151",
            "green": "10",
            "blue": "151",
            "alpha": "0",
            "label": "auto",
            "hint": "NA"
          },
          "250": {
            "red": "151",
            "green": "10",
            "blue": "151",
            "alpha": "0",
            "label": "auto",
            "hint": "distance > 4.5 km"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "invgeneralproximity",
        "compid": "invany_proximity",
        "setcolor": {
          "0": {
            "red": "151",
            "green": "10",
            "blue": "151",
            "alpha": "0",
            "label": "0",
            "hint": "no distance"
          },
          "1": {
            "red": "127",
            "green": "207",
            "blue": "237",
            "alpha": "0",
            "label": "50",
            "hint": "NA"
          },
          "55": {
            "red": "127",
            "green": "207",
            "blue": "179",
            "alpha": "0",
            "label": "1",
            "hint": "distance = 1 km"
          },
          "111": {
            "red": "127",
            "green": "207",
            "blue": "120",
            "alpha": "0",
            "label": "2",
            "hint": "distance = 2 km"
          },
          "222": {
            "red": "228",
            "green": "240",
            "blue": "120",
            "alpha": "0",
            "label": "4",
            "hint": "distance = 4 km"
          },
          "249": {
            "red": "252",
            "green": "246",
            "blue": "120",
            "alpha": "0",
            "label": "4.5",
            "hint": "NA"
          },
          "250": {
            "red": "252",
            "green": "246",
            "blue": "10",
            "alpha": "0",
            "label": "> 4.5",
            "hint": "distance > 4.5 km"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "streamproximity",
        "compid": "terrain_streamproximity",
        "setcolor": {
          "0": {
            "red": "121",
            "green": "10",
            "blue": "155",
            "alpha": "0",
            "label": "0",
            "hint": "proximity = 0"
          },
          "1": {
            "red": "127",
            "green": "107",
            "blue": "205",
            "alpha": "0",
            "label": "0",
            "hint": "NA"
          },
          "50": {
            "red": "127",
            "green": "207",
            "blue": "180",
            "alpha": "0",
            "label": "0.9",
            "hint": "distance = 900 m"
          },
          "100": {
            "red": "75",
            "green": "225",
            "blue": "130",
            "alpha": "0",
            "label": "1.8",
            "hint": "distance = 1.8 km"
          },
          "150": {
            "red": "150",
            "green": "225",
            "blue": "100",
            "alpha": "0",
            "label": "2.7",
            "hint": "distance = 2.7 km"
          },
          "200": {
            "red": "235",
            "green": "240",
            "blue": "60",
            "alpha": "0",
            "label": "3.6",
            "hint": "distance = 3.6 km"
          },
          "249": {
            "red": "252",
            "green": "130",
            "blue": "10",
            "alpha": "0",
            "label": "4.0",
            "hint": "NA"
          },
          "250": {
            "red": "190",
            "green": "100",
            "blue": "10",
            "alpha": "0",
            "label": "> 4.5",
            "hint": "distance > 4.5 km"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "hydraulhead",
        "compid": "terrain_hydraulhead",
        "setcolor": {
          "0": {
            "red": "128",
            "green": "0",
            "blue": "128",
            "alpha": "0",
            "label": "-10",
            "hint": "-10 m (cell below draining stream)"
          },
          "24": {
            "red": "64",
            "green": "0",
            "blue": "150",
            "alpha": "0",
            "label": "-1",
            "hint": "NA"
          },
          "25": {
            "red": "0",
            "green": "0",
            "blue": "187",
            "alpha": "0",
            "label": "0",
            "hint": "draining stream or water body"
          },
          "26": {
            "red": "0",
            "green": "128",
            "blue": "187",
            "alpha": "0",
            "label": "1",
            "hint": "NA"
          },
          "45": {
            "red": "128",
            "green": "255",
            "blue": "225",
            "alpha": "0",
            "label": "10",
            "hint": "10 m (above draining stream)"
          },
          "75": {
            "red": "164",
            "green": "240",
            "blue": "64",
            "alpha": "0",
            "label": "25",
            "hint": "25 m (above draining stream)"
          },
          "125": {
            "red": "248",
            "green": "238",
            "blue": "62",
            "alpha": "0",
            "label": "50",
            "hint": "50 m (above draining stream)"
          },
          "187": {
            "red": "255",
            "green": "180",
            "blue": "60",
            "alpha": "0",
            "label": "75",
            "hint": "75 m (above draining stream)"
          },
          "250": {
            "red": "255",
            "green": "200",
            "blue": "200",
            "alpha": "0",
            "label": "> 100",
            "hint": "more than 100 m above draining stream"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "divideheadold",
        "compid": "terrain_divideheadold",
        "setcolor": {
          "0": {
            "red": "128",
            "green": "0",
            "blue": "128",
            "alpha": "0",
            "label": "< -10",
            "hint": "< -10 m"
          },
          "5": {
            "red": "128",
            "green": "0",
            "blue": "128",
            "alpha": "0",
            "label": "-10",
            "hint": "NA"
          },
          "24": {
            "red": "64",
            "green": "0",
            "blue": "150",
            "alpha": "0",
            "label": "-1",
            "hint": "NA"
          },
          "25": {
            "red": "0",
            "green": "0",
            "blue": "187",
            "alpha": "0",
            "label": "0",
            "hint": "draining stream or water body"
          },
          "26": {
            "red": "0",
            "green": "128",
            "blue": "187",
            "alpha": "0",
            "label": "1",
            "hint": "NA"
          },
          "45": {
            "red": "0",
            "green": "255",
            "blue": "255",
            "alpha": "0",
            "label": "10",
            "hint": "10 m (above draining stream)"
          },
          "75": {
            "red": "255",
            "green": "255",
            "blue": "0",
            "alpha": "0",
            "label": "25",
            "hint": "25 m"
          },
          "125": {
            "red": "187",
            "green": "128",
            "blue": "0",
            "alpha": "0",
            "label": "50",
            "hint": "50 m (above draining stream)"
          },
          "187": {
            "red": "187",
            "green": "40",
            "blue": "0",
            "alpha": "0",
            "label": "75",
            "hint": "200 m (above draining stream)"
          },
          "250": {
            "red": "187",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": ">100",
            "hint": "more than 100 m above draining stream"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "dividehead",
        "compid": "terrain_dividehead",
        "setcolor": {
          "0": {
            "red": "255",
            "green": "180",
            "blue": "170",
            "alpha": "0",
            "label": "< -10",
            "hint": "< -10 m above water divide"
          },
          "25": {
            "red": "235",
            "green": "200",
            "blue": "10",
            "alpha": "0",
            "label": "0",
            "hint": "Water divide"
          },
          "26": {
            "red": "235",
            "green": "235",
            "blue": "20",
            "alpha": "0",
            "label": "1",
            "hint": "NA"
          },
          "45": {
            "red": "120",
            "green": "235",
            "blue": "120",
            "alpha": "0",
            "label": "10",
            "hint": "10 m (below water divide)"
          },
          "75": {
            "red": "0",
            "green": "235",
            "blue": "235",
            "alpha": "0",
            "label": "25",
            "hint": "25 m (below water divide)"
          },
          "125": {
            "red": "0",
            "green": "128",
            "blue": "240",
            "alpha": "0",
            "label": "50",
            "hint": "50 m (below water divide)"
          },
          "187": {
            "red": "0",
            "green": "15",
            "blue": "240",
            "alpha": "0",
            "label": "75",
            "hint": "75m (below water divide)"
          },
          "250": {
            "red": "0",
            "green": "0",
            "blue": "169",
            "alpha": "0",
            "label": ">100",
            "hint": "more than 100 m below water divide"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "tci",
        "compid": "terrain_tci",
        "setcolor": {
          "0": {
            "red": "166",
            "green": "37",
            "blue": "39",
            "alpha": "0",
            "label": "0",
            "hint": "TCI = 0"
          },
          "1": {
            "red": "215",
            "green": "50",
            "blue": "45",
            "alpha": "0",
            "label": "0.2",
            "hint": "NA"
          },
          "20": {
            "red": "245",
            "green": "173",
            "blue": "96",
            "alpha": "0",
            "label": "5.0",
            "hint": "TCI = 5"
          },
          "70": {
            "red": "252",
            "green": "224",
            "blue": "144",
            "alpha": "0",
            "label": "10",
            "hint": "TCI = 10"
          },
          "120": {
            "red": "171",
            "green": "217",
            "blue": "171",
            "alpha": "0",
            "label": "15",
            "hint": "TCI = 15"
          },
          "170": {
            "red": "71",
            "green": "117",
            "blue": "220",
            "alpha": "0",
            "label": "20",
            "hint": "TCI = 20"
          },
          "220": {
            "red": "50",
            "green": "75",
            "blue": "170",
            "alpha": "0",
            "label": "25",
            "hint": "TCI = 25"
          },
          "250": {
            "red": "19",
            "green": "24",
            "blue": "120",
            "alpha": "0",
            "label": "> 28",
            "hint": "TCI > 28"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "updrain",
        "compid": "terrain_updrain",
        "setcolor": {
          "0": {
            "red": "200",
            "green": "37",
            "blue": "39",
            "alpha": "0",
            "label": "0.01",
            "hint": "0.01 km2"
          },
          "1": {
            "red": "215",
            "green": "50",
            "blue": "45",
            "alpha": "0",
            "label": "1",
            "hint": "NA"
          },
          "10": {
            "red": "245",
            "green": "173",
            "blue": "96",
            "alpha": "0",
            "label": "0.02",
            "hint": "NA"
          },
          "22": {
            "red": "252",
            "green": "245",
            "blue": "120",
            "alpha": "0",
            "label": "0.05",
            "hint": "0.05 km2"
          },
          "50": {
            "red": "171",
            "green": "207",
            "blue": "120",
            "alpha": "0",
            "label": "0.5",
            "hint": "0.5 km2"
          },
          "124": {
            "red": "121",
            "green": "167",
            "blue": "170",
            "alpha": "0",
            "label": "250",
            "hint": "250 km2"
          },
          "187": {
            "red": "51",
            "green": "117",
            "blue": "220",
            "alpha": "0",
            "label": "50000",
            "hint": "500000 km2"
          },
          "250": {
            "red": "21",
            "green": "34",
            "blue": "170",
            "alpha": "0",
            "label": "> 9000000",
            "hint": "> 9000000 km2"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "NA"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "NA"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "spi",
        "compid": "terrain_spi",
        "setcolor": {
          "0": {
            "red": "180",
            "green": "180",
            "blue": "173",
            "alpha": "0",
            "label": "0",
            "hint": "0"
          },
          "20": {
            "red": "230",
            "green": "230",
            "blue": "173",
            "alpha": "0",
            "label": "3.0",
            "hint": "SPI = 3"
          },
          "80": {
            "red": "171",
            "green": "217",
            "blue": "255",
            "alpha": "0",
            "label": "50",
            "hint": "SPI = 50"
          },
          "160": {
            "red": "69",
            "green": "117",
            "blue": "180",
            "alpha": "0",
            "label": "3000",
            "hint": "SPI = 3000"
          },
          "250": {
            "red": "169",
            "green": "54",
            "blue": "149",
            "alpha": "0",
            "label": "> 250000",
            "hint": "log (SPI) > 250000"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "ruslelfactor",
        "compid": "terrain_ruslelfactor",
        "setcolor": {
          "0": {
            "red": "75",
            "green": "75",
            "blue": "125",
            "alpha": "0",
            "label": "0",
            "hint": "RUSLE L factor = 0"
          },
          "1": {
            "red": "75",
            "green": "116",
            "blue": "67",
            "alpha": "0",
            "label": "0",
            "hint": "NA"
          },
          "2": {
            "red": "127",
            "green": "207",
            "blue": "120",
            "alpha": "0",
            "label": "0",
            "hint": "NA"
          },
          "25": {
            "red": "252",
            "green": "245",
            "blue": "120",
            "alpha": "0",
            "label": "1.0",
            "hint": "RUSLE L factor = 1.0"
          },
          "125": {
            "red": "252",
            "green": "145",
            "blue": "60",
            "alpha": "0",
            "label": "5.0",
            "hint": "RUSLE L factor = 5.0"
          },
          "200": {
            "red": "170",
            "green": "70",
            "blue": "23",
            "alpha": "0",
            "label": "8.0",
            "hint": "RUSLE L factor = 8.0"
          },
          "249": {
            "red": "161",
            "green": "43",
            "blue": "161",
            "alpha": "0",
            "label": "10",
            "hint": "NA"
          },
          "250": {
            "red": "161",
            "green": "10",
            "blue": "151",
            "alpha": "0",
            "label": "> 10",
            "hint": "RUSLE L factor >= 10"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "slopelength",
        "compid": "terrain_slopelength",
        "setcolor": {
          "0": {
            "red": "128",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "slope",
            "hint": "slopee"
          },
          "1": {
            "red": "255",
            "green": "128",
            "blue": "0",
            "alpha": "0",
            "label": "slope",
            "hint": "slopee"
          },
          "20": {
            "red": "128",
            "green": "255",
            "blue": "128",
            "alpha": "0",
            "label": "slope",
            "hint": "slope"
          },
          "125": {
            "red": "0",
            "green": "128",
            "blue": "187",
            "alpha": "0",
            "label": "slope",
            "hint": "slope"
          },
          "250": {
            "red": "0",
            "green": "0",
            "blue": "128",
            "alpha": "0",
            "label": "flat",
            "hint": "flat"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "ruslesfactor",
        "compid": "terrain_ruslesfactor",
        "setcolor": {
          "0": {
            "red": "64",
            "green": "128",
            "blue": "164",
            "alpha": "0",
            "label": "0",
            "hint": "RUSLE S factor = 0"
          },
          "1": {
            "red": "0",
            "green": "187",
            "blue": "128",
            "alpha": "0",
            "label": "1",
            "hint": "NA"
          },
          "50": {
            "red": "255",
            "green": "255",
            "blue": "0",
            "alpha": "0",
            "label": "1.0",
            "hint": "RUSLE S factor = 1.0"
          },
          "150": {
            "red": "255",
            "green": "128",
            "blue": "0",
            "alpha": "0",
            "label": "3.0",
            "hint": "RUSLE S factor = 3.0"
          },
          "250": {
            "red": "128",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "> 5.0",
            "hint": "RUSLE S factor > 5.0"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "slopesteepness",
        "compid": "terrain_slopesteepness",
        "setcolor": {
          "0": {
            "red": "64",
            "green": "128",
            "blue": "164",
            "alpha": "0",
            "label": "slope",
            "hint": "slope"
          },
          "1": {
            "red": "0",
            "green": "187",
            "blue": "128",
            "alpha": "0",
            "label": "slope",
            "hint": "slope"
          },
          "87": {
            "red": "255",
            "green": "255",
            "blue": "0",
            "alpha": "0",
            "label": "slope",
            "hint": "slope"
          },
          "168": {
            "red": "255",
            "green": "128",
            "blue": "0",
            "alpha": "0",
            "label": "slope",
            "hint": "slope"
          },
          "250": {
            "red": "128",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "slope",
            "hint": "slopee"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "demcurvature",
        "compid": "dem_pcurve",
        "setcolor": {
          "0": {
            "red": "0",
            "green": "0",
            "blue": "128",
            "alpha": "0",
            "label": "strongly concave",
            "hint": "strongly concave"
          },
          "62": {
            "red": "0",
            "green": "128",
            "blue": "255",
            "alpha": "0",
            "label": "moderately concave",
            "hint": "moderately concave"
          },
          "125": {
            "red": "232",
            "green": "232",
            "blue": "232",
            "alpha": "0",
            "label": "planar",
            "hint": "planar"
          },
          "187": {
            "red": "255",
            "green": "128",
            "blue": "0",
            "alpha": "0",
            "label": "moderately convex",
            "hint": "Moderately convex"
          },
          "250": {
            "red": "128",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "strongly convex",
            "hint": "strongly convex"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "tpi",
        "compid": "dem_tpi",
        "setcolor": {
          "0": {
            "red": "0",
            "green": "0",
            "blue": "128",
            "alpha": "0",
            "label": "< -25",
            "hint": "TPI <= -25"
          },
          "75": {
            "red": "0",
            "green": "128",
            "blue": "255",
            "alpha": "0",
            "label": "-10",
            "hint": "TPI = -10"
          },
          "125": {
            "red": "232",
            "green": "232",
            "blue": "232",
            "alpha": "0",
            "label": "0",
            "hint": "TPI = 0"
          },
          "175": {
            "red": "255",
            "green": "128",
            "blue": "0",
            "alpha": "0",
            "label": "10",
            "hint": "TPI = 10"
          },
          "250": {
            "red": "128",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "> 25",
            "hint": "TPI >= 25"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "tri",
        "compid": "dem_tri",
        "setcolor": {
          "0": {
            "red": "44",
            "green": "143",
            "blue": "168",
            "alpha": "0",
            "label": "0 (flat)",
            "hint": "flat"
          },
          "5": {
            "red": "30",
            "green": "182",
            "blue": "130",
            "alpha": "0",
            "label": "1",
            "hint": "NA"
          },
          "50": {
            "red": "190",
            "green": "210",
            "blue": "40",
            "alpha": "0",
            "label": "10",
            "hint": "tri=10"
          },
          "100": {
            "red": "255",
            "green": "255",
            "blue": "7",
            "alpha": "0",
            "label": "20",
            "hint": "tri=20"
          },
          "150": {
            "red": "250",
            "green": "192",
            "blue": "3",
            "alpha": "0",
            "label": "30",
            "hint": "tri=30"
          },
          "200": {
            "red": "243",
            "green": "128",
            "blue": "0",
            "alpha": "0",
            "label": "40",
            "hint": "tri=40"
          },
          "250": {
            "red": "145",
            "green": "33",
            "blue": "8",
            "alpha": "0",
            "label": ">=50",
            "hint": "tri >=50"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "tri2",
        "compid": "dem_tri2",
        "setcolor": {
          "0": {
            "red": "44",
            "green": "143",
            "blue": "168",
            "alpha": "0",
            "label": "0 (flat)",
            "hint": "flat"
          },
          "5": {
            "red": "90",
            "green": "182",
            "blue": "130",
            "alpha": "0",
            "label": "1",
            "hint": "NA"
          },
          "50": {
            "red": "205",
            "green": "210",
            "blue": "105",
            "alpha": "0",
            "label": "10",
            "hint": "tri=10"
          },
          "100": {
            "red": "253",
            "green": "253",
            "blue": "155",
            "alpha": "0",
            "label": "20",
            "hint": "tri=20"
          },
          "150": {
            "red": "250",
            "green": "206",
            "blue": "73",
            "alpha": "0",
            "label": "30",
            "hint": "tri=30"
          },
          "200": {
            "red": "243",
            "green": "164",
            "blue": "80",
            "alpha": "0",
            "label": "40",
            "hint": "tri=40"
          },
          "250": {
            "red": "207",
            "green": "91",
            "blue": "68",
            "alpha": "0",
            "label": ">=50",
            "hint": "tri >=50"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "shade",
        "compid": "dem_shade",
        "setcolor": {
          "0": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "0",
            "hint": "Complete shade"
          },
          "250": {
            "red": "255",
            "green": "255",
            "blue": "255",
            "alpha": "0",
            "label": "250",
            "hint": "complete light"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "globaldem",
        "compid": "dem_dem",
        "setcolor": {
          "0": {
            "red": "80",
            "green": "150",
            "blue": "91",
            "alpha": "0",
            "label": "0",
            "hint": "Sea level"
          },
          "125": {
            "red": "235",
            "green": "245",
            "blue": "220",
            "alpha": "0",
            "label": "4000",
            "hint": "4000 masl"
          },
          "250": {
            "red": "220",
            "green": "133",
            "blue": "60",
            "alpha": "0",
            "label": "4000",
            "hint": "4000 masl"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "shadedem",
        "compid": "shadedem_dem",
        "setcolor": {
          "0": {
            "red": "122",
            "green": "200",
            "blue": "91",
            "alpha": "0",
            "label": "0",
            "hint": "Sea level"
          },
          "125": {
            "red": "255",
            "green": "255",
            "blue": "200",
            "alpha": "0",
            "label": "4000",
            "hint": "4000 masl"
          },
          "250": {
            "red": "220",
            "green": "133",
            "blue": "60",
            "alpha": "0",
            "label": "4000",
            "hint": "4000 masl"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "fullrangedem",
        "compid": "fullrangedem_dem",
        "setcolor": {
          "0": {
            "red": "0",
            "green": "101",
            "blue": "29",
            "alpha": "0",
            "label": "0",
            "hint": "Sea level"
          },
          "125": {
            "red": "252",
            "green": "255",
            "blue": "0",
            "alpha": "0",
            "label": "4000",
            "hint": "4000 masl"
          },
          "225": {
            "red": "139",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "4000",
            "hint": "4000 masl"
          },
          "250": {
            "red": "242",
            "green": "233",
            "blue": "237",
            "alpha": "0",
            "label": "4000",
            "hint": "4000 masl"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "upland drainage",
            "hint": "upland drainage"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "dem_darkest_fixed",
        "compid": "dem_darkest_fixed",
        "setcolor": {
          "0": {
            "red": "41",
            "green": "96",
            "blue": "58",
            "alpha": "0",
            "label": "0",
            "hint": "Sea level"
          },
          "25": {
            "red": "54",
            "green": "121",
            "blue": "36",
            "alpha": "0",
            "label": "800",
            "hint": "800 masl"
          },
          "125": {
            "red": "247",
            "green": "248",
            "blue": "80",
            "alpha": "0",
            "label": "4000",
            "hint": "4000 masl"
          },
          "225": {
            "red": "121",
            "green": "24",
            "blue": "21",
            "alpha": "0",
            "label": "7200",
            "hint": "7200 masl"
          },
          "250": {
            "red": "250",
            "green": "240",
            "blue": "245",
            "alpha": "0",
            "label": ">= 8000",
            "hint": ">= 8000 masl"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "NA",
            "hint": "NA"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "No data",
            "hint": "No data"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "dem_dark_fixed",
        "compid": "dem_dark_fixed",
        "setcolor": {
          "0": {
            "red": "54",
            "green": "121",
            "blue": "36",
            "alpha": "0",
            "label": "0",
            "hint": "Sea level"
          },
          "125": {
            "red": "247",
            "green": "248",
            "blue": "80",
            "alpha": "0",
            "label": "4000",
            "hint": "4000 masl"
          },
          "250": {
            "red": "121",
            "green": "24",
            "blue": "21",
            "alpha": "0",
            "label": ">= 8000",
            "hint": ">= 8000 masl"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "MA",
            "hint": "MA"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "No data",
            "hint": "No data"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "dem_darkest_auto",
        "compid": "dem_darkest_auto",
        "setcolor": {
          "0": {
            "red": "41",
            "green": "96",
            "blue": "58",
            "alpha": "0",
            "label": "auto",
            "hint": "auto"
          },
          "25": {
            "red": "54",
            "green": "121",
            "blue": "36",
            "alpha": "0",
            "label": "auto",
            "hint": "auto"
          },
          "125": {
            "red": "247",
            "green": "248",
            "blue": "80",
            "alpha": "0",
            "label": "auto",
            "hint": "auto"
          },
          "225": {
            "red": "121",
            "green": "24",
            "blue": "21",
            "alpha": "0",
            "label": "auto",
            "hint": "auto"
          },
          "250": {
            "red": "250",
            "green": "240",
            "blue": "245",
            "alpha": "0",
            "label": "auto",
            "hint": "auto"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "NA",
            "hint": "NA"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "No data",
            "hint": "NA"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "dem_light_fixed",
        "compid": "dem_light_fixed",
        "setcolor": {
          "0": {
            "red": "90",
            "green": "135",
            "blue": "75",
            "alpha": "0",
            "label": "0",
            "hint": "Sea level"
          },
          "63": {
            "red": "230",
            "green": "219",
            "blue": "165",
            "alpha": "0",
            "label": "2000",
            "hint": "2000 masl"
          },
          "125": {
            "red": "250",
            "green": "200",
            "blue": "110",
            "alpha": "0",
            "label": "4000",
            "hint": "4000 masl"
          },
          "184": {
            "red": "184",
            "green": "157",
            "blue": "139",
            "alpha": "0",
            "label": "6000",
            "hint": "6000 masl"
          },
          "250": {
            "red": "252",
            "green": "249",
            "blue": "245",
            "alpha": "0",
            "label": ">= 8000",
            "hint": ">= 8000 masl"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "NA",
            "hint": "NA"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "No data",
            "hint": "No data"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "dem_light_auto",
        "compid": "dem_light_auto",
        "setcolor": {
          "0": {
            "red": "90",
            "green": "135",
            "blue": "75",
            "alpha": "0",
            "label": "auto",
            "hint": "auto"
          },
          "62": {
            "red": "230",
            "green": "219",
            "blue": "165",
            "alpha": "0",
            "label": "auto",
            "hint": "auto"
          },
          "125": {
            "red": "250",
            "green": "200",
            "blue": "110",
            "alpha": "0",
            "label": "auto",
            "hint": "auto"
          },
          "183": {
            "red": "184",
            "green": "157",
            "blue": "139",
            "alpha": "0",
            "label": "auto",
            "hint": "auto"
          },
          "250": {
            "red": "252",
            "green": "249",
            "blue": "245",
            "alpha": "0",
            "label": "auto",
            "hint": "auto"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "NA",
            "hint": "NA"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "No data",
            "hint": "No data"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "dem_lightest_fixed",
        "compid": "dem_lightest_fixed",
        "setcolor": {
          "0": {
            "red": "148",
            "green": "188",
            "blue": "114",
            "alpha": "0",
            "label": "0",
            "hint": "Sea level"
          },
          "125": {
            "red": "255",
            "green": "252",
            "blue": "207",
            "alpha": "0",
            "label": "4000",
            "hint": "4000 masl"
          },
          "250": {
            "red": "244",
            "green": "158",
            "blue": "95",
            "alpha": "0",
            "label": ">= 8000",
            "hint": ">= 8000 masl"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "NA",
            "hint": "NA"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "No data",
            "hint": "No data"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "dem_lightest_auto",
        "compid": "dem_lightest_auto",
        "setcolor": {
          "0": {
            "red": "148",
            "green": "188",
            "blue": "114",
            "alpha": "0",
            "label": "auto",
            "hint": "auto"
          },
          "125": {
            "red": "255",
            "green": "252",
            "blue": "207",
            "alpha": "0",
            "label": "auto",
            "hint": "auto"
          },
          "250": {
            "red": "244",
            "green": "158",
            "blue": "95",
            "alpha": "0",
            "label": "auto",
            "hint": "auto"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "NA",
            "hint": "NA"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "No data",
            "hint": "No data"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "geomorphon",
        "compid": "dem_geomorphon",
        "setcolor": {
          "0": {
            "red": "255",
            "green": "255",
            "blue": "255",
            "alpha": "0",
            "label": "NA",
            "hint": "unused"
          },
          "1": {
            "red": "220",
            "green": "220",
            "blue": "220",
            "alpha": "0",
            "label": "flat",
            "hint": "flat"
          },
          "2": {
            "red": "121",
            "green": "5",
            "blue": "4",
            "alpha": "0",
            "label": "summit",
            "hint": "summit (2)"
          },
          "3": {
            "red": "186",
            "green": "42",
            "blue": "37",
            "alpha": "0",
            "label": "ridge",
            "hint": "ridge (3)"
          },
          "4": {
            "red": "237",
            "green": "93",
            "blue": "58",
            "alpha": "0",
            "label": "shoulder",
            "hint": "shouldr (4)"
          },
          "5": {
            "red": "246",
            "green": "207",
            "blue": "91",
            "alpha": "0",
            "label": "spur",
            "hint": "spur (5)"
          },
          "6": {
            "red": "255",
            "green": "249",
            "blue": "99",
            "alpha": "0",
            "label": "slope",
            "hint": "slope (6)"
          },
          "7": {
            "red": "191",
            "green": "222",
            "blue": "70",
            "alpha": "0",
            "label": "hollow",
            "hint": "hollow (7)"
          },
          "8": {
            "red": "123",
            "green": "241",
            "blue": "155",
            "alpha": "0",
            "label": "footslope",
            "hint": "footslope (8)"
          },
          "9": {
            "red": "0",
            "green": "69",
            "blue": "245",
            "alpha": "0",
            "label": "valley",
            "hint": "valley (9)"
          },
          "10": {
            "red": "30",
            "green": "8",
            "blue": "60",
            "alpha": "0",
            "label": "depression",
            "hint": "depression (10)"
          },
          "250": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "NA",
            "hint": "extra"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "NA",
            "hint": "extra"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "NA",
            "hint": "extra"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "geomorphlegend",
        "compid": "dem_geomorphlegend",
        "setcolor": {
          "5": {
            "red": "220",
            "green": "235",
            "blue": "240",
            "alpha": "0",
            "label": "plain",
            "hint": "NA"
          },
          "10": {
            "red": "220",
            "green": "235",
            "blue": "240",
            "alpha": "0",
            "label": "plain",
            "hint": "plain or flat"
          },
          "11": {
            "red": "180",
            "green": "20",
            "blue": "10",
            "alpha": "0",
            "label": "peak",
            "hint": "NA"
          },
          "20": {
            "red": "180",
            "green": "20",
            "blue": "10",
            "alpha": "0",
            "label": "peak",
            "hint": "peak or summit"
          },
          "21": {
            "red": "255",
            "green": "128",
            "blue": "10",
            "alpha": "0",
            "label": "ridge",
            "hint": "NA"
          },
          "30": {
            "red": "255",
            "green": "128",
            "blue": "10",
            "alpha": "0",
            "label": "ridge",
            "hint": "lodal ridge"
          },
          "31": {
            "red": "235",
            "green": "205",
            "blue": "15",
            "alpha": "0",
            "label": "upper slope, shoulder",
            "hint": "NA"
          },
          "40": {
            "red": "235",
            "green": "205",
            "blue": "15",
            "alpha": "0",
            "label": "upper slope,shoulder",
            "hint": "upper slope,shoulder"
          },
          "41": {
            "red": "224",
            "green": "80",
            "blue": "80",
            "alpha": "0",
            "label": "spur",
            "hint": "NA"
          },
          "50": {
            "red": "224",
            "green": "80",
            "blue": "80",
            "alpha": "0",
            "label": "spur",
            "hint": "spur"
          },
          "51": {
            "red": "230",
            "green": "230",
            "blue": "120",
            "alpha": "0",
            "label": "open slope",
            "hint": "NA"
          },
          "60": {
            "red": "230",
            "green": "230",
            "blue": "120",
            "alpha": "0",
            "label": "open slope",
            "hint": "open slope"
          },
          "61": {
            "red": "25",
            "green": "155",
            "blue": "234",
            "alpha": "0",
            "label": "hollow",
            "hint": "NA"
          },
          "70": {
            "red": "25",
            "green": "155",
            "blue": "234",
            "alpha": "0",
            "label": "hollow",
            "hint": "hollow"
          },
          "71": {
            "red": "0",
            "green": "128",
            "blue": "128",
            "alpha": "0",
            "label": "U-shaped valley or footslope",
            "hint": "NA"
          },
          "80": {
            "red": "0",
            "green": "128",
            "blue": "128",
            "alpha": "0",
            "label": "U-shaped valley or footslope",
            "hint": "U-shaped valley or footslope"
          },
          "81": {
            "red": "10",
            "green": "160",
            "blue": "10",
            "alpha": "0",
            "label": "midslope/shallow valley, hollow",
            "hint": "NA"
          },
          "90": {
            "red": "10",
            "green": "160",
            "blue": "10",
            "alpha": "0",
            "label": "midslope/shallow valley, hollow",
            "hint": "midslope/shallow valley, hollow"
          },
          "91": {
            "red": "30",
            "green": "0",
            "blue": "170",
            "alpha": "0",
            "label": "Depression, canyon or valley",
            "hint": "NA"
          },
          "100": {
            "red": "30",
            "green": "0",
            "blue": "170",
            "alpha": "0",
            "label": "Depression, canyon or valley",
            "hint": "Depression, canyon or valley"
          },
          "105": {
            "red": "30",
            "green": "0",
            "blue": "170",
            "alpha": "0",
            "label": "Depression, canyon or valley",
            "hint": "NA"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "NA",
            "hint": "NA"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "NA",
            "hint": "NA"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "ps-morphology",
        "compid": "dem_ps-geomorphology",
        "setcolor": {
          "0": {
            "red": "255",
            "green": "255",
            "blue": "255",
            "alpha": "0",
            "label": "NA",
            "hint": "unused"
          },
          "3": {
            "red": "0",
            "green": "69",
            "blue": "245",
            "alpha": "0",
            "label": "valley/channel",
            "hint": "valley/chanel (3)"
          },
          "4": {
            "red": "191",
            "green": "222",
            "blue": "70",
            "alpha": "0",
            "label": "hollow/pass",
            "hint": "hollow/pass (4)"
          },
          "5": {
            "red": "246",
            "green": "207",
            "blue": "91",
            "alpha": "0",
            "label": "ridge/spur",
            "hint": "ridge/spur(5)"
          },
          "6": {
            "red": "121",
            "green": "5",
            "blue": "4",
            "alpha": "0",
            "label": "peak/summit",
            "hint": "peak/summit (6)"
          },
          "10": {
            "red": "220",
            "green": "220",
            "blue": "220",
            "alpha": "0",
            "label": "flat",
            "hint": "flat"
          },
          "22": {
            "red": "30",
            "green": "8",
            "blue": "60",
            "alpha": "0",
            "label": "depression/pit",
            "hint": "depression/pit (2)"
          },
          "250": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "NA",
            "hint": "extra"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "NA",
            "hint": "extra"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "NA",
            "hint": "extra"
          }
        }
      }
    },
    {
      "processid": "AddRasterPalette",
      "overwrite": false,
      "parameters": {
        "palette": "ps-morphology-legend",
        "compid": "dem_ps-geomorphology-legend",
        "setcolor": {
          "5": {
            "red": "220",
            "green": "235",
            "blue": "240",
            "alpha": "0",
            "label": "plain",
            "hint": "NA"
          },
          "10": {
            "red": "220",
            "green": "235",
            "blue": "240",
            "alpha": "0",
            "label": "plain",
            "hint": "plain or flat"
          },
          "11": {
            "red": "30",
            "green": "0",
            "blue": "170",
            "alpha": "0",
            "label": "depression/pit",
            "hint": "NA"
          },
          "20": {
            "red": "30",
            "green": "0",
            "blue": "170",
            "alpha": "0",
            "label": "depression/pit",
            "hint": "depression/pit (2)"
          },
          "21": {
            "red": "0",
            "green": "128",
            "blue": "128",
            "alpha": "0",
            "label": "valley/channel",
            "hint": "NA"
          },
          "30": {
            "red": "0",
            "green": "128",
            "blue": "128",
            "alpha": "0",
            "label": "valley/channel",
            "hint": "valley/chanel (3)"
          },
          "31": {
            "red": "25",
            "green": "155",
            "blue": "234",
            "alpha": "0",
            "label": "hollow/pass",
            "hint": "NA"
          },
          "40": {
            "red": "25",
            "green": "155",
            "blue": "234",
            "alpha": "0",
            "label": "hollow/pass",
            "hint": "hollow/pass (4)"
          },
          "41": {
            "red": "255",
            "green": "128",
            "blue": "10",
            "alpha": "0",
            "label": "ridge/spur",
            "hint": "NA"
          },
          "50": {
            "red": "255",
            "green": "128",
            "blue": "10",
            "alpha": "0",
            "label": "ridge/spur",
            "hint": "ridge/spur(5)"
          },
          "51": {
            "red": "180",
            "green": "20",
            "blue": "10",
            "alpha": "0",
            "label": "peak/summit",
            "hint": "NA"
          },
          "60": {
            "red": "180",
            "green": "20",
            "blue": "10",
            "alpha": "0",
            "label": "peak/summit",
            "hint": "peak/summit (6)"
          },
          "65": {
            "red": "180",
            "green": "20",
            "blue": "10",
            "alpha": "0",
            "label": "peak/summit",
            "hint": "NA"
          },
          "251": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "NA",
            "hint": "NA"
          },
          "255": {
            "red": "0",
            "green": "0",
            "blue": "0",
            "alpha": "0",
            "label": "NA",
            "hint": "NA"
          }
        }
      }
    }
  ]
}
```
