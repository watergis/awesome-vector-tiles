# awesome-vector-tiles

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![Gitter](https://badges.gitter.im/narwassco/community.svg)](https://gitter.im/narwassco/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

This is awesome implementations of the Mapbox Vector Tile for Water Services Providers.

## This repository is no longer used, it has been moved to [watergis/docs](https://github.com/watergis/docs) repository!

Please visit [https://docs.water-gis.com](https://docs.water-gis.com) for the latest documentation.

---
## Why Vectortiles?

> Vector tiles make huge maps fast while offering full design flexibility. They are the vector data equivalent of image tiles for web mapping, applying the strengths of tiling — developed for caching, scaling and serving map imagery rapidly — to vector data. (from [Mapbox website](https://docs.mapbox.com/vector-tiles/reference/)).

`Vectortiles` is the most popular and advanced mapping technology currently, its data is very light and fast, offering full design flexibility. 

Its operation cost is normally cheaper compare to raster tiles data distribution.

In Africa, Internet connection is still poor in some rural area. This vectortiles is right solution for such as poor internet situation. You can enjoy browsing smoothly in your computer or smartphones.

Our vectortiles approach uses Github pages without servers. I know it is quite difficult for some of water services providers to have servers in Africa. This toolkits were developed for you!

---
## Steps for implementation of Vectortiles

1. [Requirements before setup](./contents/requirements.md)

2. [How to generate vector tiles](./contents/how-to-generate-vectortiles.md)

3. [Cost of Operation & Maintenance for Vectortiles](./contents/costs.md)

---
## Use Cases

The following websites are the final outputs of vector tiles maps for water sevices providers in both Kenya and Rwanda which are using this vector tiles toolkit.

1. [Water Supply Map for Narok Water, KENYA](https://narok.water-gis.com): since June 2020.
2. [Water Supply Map for WASAC RWSS, RWANDA](https://rural.water-gis.com): since July 2020.
3. [Water Supply Map for Nakuru Water, KENYA](https://nakuru.water-gis.com): since August 2020.

The below is demo image of `Water Supply Map for WASAC RWSS`

![demo](./images/demo_wasac.gif)

You will see how this vectortiles is powerful for your water services providers.

## Overview map
I developed an [overview map](https://watergis.github.io/water-map) for to manage all of vectortiles of water supply system. You can zoom the map and tap any point, so you can see more detailed water supply network data from the link of popup.

![image](https://user-images.githubusercontent.com/2639701/91636570-a8d9ba00-ea3c-11ea-924c-383725a297ca.png)

## Lincense

### 1. Source Code
All the source codes under `watergis` organization are open source software, they are mostly [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT). 

<details>
<summary>List of All repositories under watergis</summary>

#### a. Software for Mapbox GL JS client
- [watergis/mapbox-gl-legend](https://github.com/watergis/mapbox-gl-legend): Add a simple legend control
- [watergis/mapbox-gl-area-switcher](https://github.com/watergis/mapbox-gl-area-switcher): Add a simple control to switch area easier
- [watergis/mapbox-gl-popup](https://github.com/watergis/mapbox-gl-popup): add a simple popup into Mapbox GL JS.
- [watergis/mapbox-gl-print](https://github.com/watergis/mapbox-gl-print): add a simple print control to export PNG and PDF.
- [watergis/mapbox-gl-pitch-toggle-control](https://github.com/watergis/mapbox-gl-pitch-toggle-control): add a simple 3D button to change between 3D and 2D

#### b. Software for Vectortiles
- [watergis/vt-boilerplate](https://github.com/watergis/vt-boilerplate): a template to create vectortiles from PostGIS and deploy it to Github pages.
- [watergis/postgis2geojson](https://github.com/watergis/postgis2geojson): a module to extract GeoJSON directly from PostGIS.
- [watergis/postgis2mbtiles](https://github.com/watergis/postgis2mbtiles): a module to extract mbtiles directly from PostGIS.
- [watergis/postgis2mbtiles-docker](https://github.com/watergis/postgis2mbtiles-docker): a Docker implementation for `postgis2mbtiles` module.
- [watergis/mbtiles2pbf](https://github.com/watergis/mbtiles2pbf): a module to convert from mbtiles to pbf(mvt) vectortiles.
- [watergis/postgis2vectortiles](https://github.com/watergis/postgis2vectortiles): a module to create pbf vectortiles from PostGIS directly.
- [watergis/sprite-creator](https://github.com/watergis/sprite-creator): a module to create sprite files from SVG icons.

#### c. Software for EPANET
- [watergis/geojson2inp](https://github.com/watergis/geojson2inp): a module create INP file from GeoJSON files.
- [watergis/postgis2inp](https://github.com/watergis/postgis2inp): a module create INP file directly from PostGIS.

These repositories are not currently related to vectortiles, however I would like to develop EPANET functions within vectortiles map in the future.

</details>

### 2. Vector tile
Actual vectortiles datas are owned by their water companies. Vectortiles data are located in following repositories.

- [narwassco/vt](https://github.com/narwassco/vt): Vectortiles for Narok Water, Kenya
- [WASAC/vt](https://github.com/WASAC/vt): Vectortiles for WASAC, Rwanda
- [nakuruwater/vt](https://github.com/nakuruwater/vt): Vectortiles for Nakuru Water, Kenya

Those vectortiles are licensed under a [Creative Commons Attribution 4.0 International
License](http://creativecommons.org/licenses/by/4.0/)([![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)).

If you want to use their open data, please mention their attiribution. For instance,

- Attribution of Narok Water, Kenya
```
Copyright (c) 2020 Narok Water and Serwerage Services Co, Ltd.
```
- Atribution of WASAC, Rwanda
```
Copyright (c) 2020 Water and Sanitation Corporation, Ltd.
```
- Attribution of Nakuru Water, Kenya
```
Copyright (c) 2020 Nakuru Water and Sanitation Services Co, Ltd.
```

Also, if you want to use our stylefiles together with base map, please put the following additional attribution on your map.

```
(c)Mapbox, (c) OpenStreetMap contributors, Powered by the United Nations Vector Tile Toolkit
```

### 3. Stylefiles and Spritefiles
Those stylefiles and spritefiles are following [Mapbox Style Specification](https://docs.mapbox.com/mapbox-gl-js/style-spec/). The repositories are as follows.

- [narwassco/mapbox-stylefiles](https://github.com/narwassco/mapbox-stylefiles): Stylefiles for Narok Water, Kenya
- [WASAC/mapbox-stylefiles](https://github.com/WASAC/mapbox-stylefiles): Stylefiles for WASAC, Rwanda.
- [nakuruwater/mapbox-stylefiles](https://github.com/nakuruwater/mapbox-stylefiles): Stylefiles for Nakuru Water, Kenya

Those stylefiles are licenced under `C0-1.0 License`. However, we are using some icons of Mapbox Studio. So those icons which are from Mapbox, the license also belong them.


---
## Contributions

This vectortiles toolkit was developed and is maintained by Jin IGARASHI(see [portfolio](https://water-gis.com) if you are fascinated by more details about me). If you have any feedbacks, please let me know through Github's issues or pull request. Also, if you like my GIS works for water services providers in Africa, you can make donation through [Github Sponsor](https://github.com/sponsors/JinIgarashi).

---
`Copyright © 2020 Jin IGARASHI`
