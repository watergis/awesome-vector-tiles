# awesome-vector-tiles
This is awesome implementations of the Mapbox Vector Tile for Water Services Providers.

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

1. [Water Supply Map for Narok Water, KENYA](https://narok.water-gis.com)
2. [Water Supply Map for WASAC RWSS, RWANDA](https://rural.water-gis.com)

The below is demo image of `Water Supply Map for WASAC RWSS`

![demo](./images/demo_wasac.gif)

You will see how this vectortiles is powerful for your water services providers.

## Lincense

### 1. Source Code
All the source codes under `watergis` organization are open source software, they are mostly `MIT license`. 

<details>
<summary>List of All repositories under watergis</summary>

#### a. Software for Mapbox GL JS client
- [watergis/mapbox-gl-legend](https://github.com/watergis/mapbox-gl-legend): Add a simple legend control
- [watergis/mapbox-gl-area-switcher](https://github.com/watergis/mapbox-gl-area-switcher): Add a simple control to switch area easier
- [watergis/mapbox-gl-popup](https://github.com/watergis/mapbox-gl-popup): add a simple popup into Mapbox GL JS.
- [watergis/mapbox-gl-print](https://github.com/watergis/mapbox-gl-print): add a simple print control to export PNG and PDF.
- [watergis/mapbox-gl-pitch-toggle-control](https://github.com/watergis/mapbox-gl-pitch-toggle-control): add a simple 3D button to change between 3D and 2D

#### b. Software for Vectortiles
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
Shield: [![CC BY 4.0][cc-by-shield]][cc-by]

Actual vectortiles datas are owned by their water companies. Vectortiles data are located in following repositories.

- [WASAC/vt](https://github.com/WASAC/vt): Vectortiles for WASAC, Rwanda
- [narwassco/vt](https://github.com/WASAC/vt): Vectortiles for Narok Water, Kenya

Those vectortiles are licensed under a [Creative Commons Attribution 4.0 International
License](http://creativecommons.org/licenses/by/4.0/).

If you want to use their open data, please mention their attiribution. For instance,

- Attribution of Narok Water, Kenya
```
Copyright (c) 2020 Narok Water and Serwerage Services Co, Ltd.
```
- Atribution of WASAC, Rwanda
```
Copyright (c) 2020 Water and Sanitation Corporation, Ltd.
```

### 3. Stylefiles and Spritefiles

Those stylefiles and spritefiles are following [Mapbox Style Specification](https://docs.mapbox.com/mapbox-gl-js/style-spec/). The repositories are as follows.

- [narwassco/mapbox-stylefiles](https://github.com/narwassco/mapbox-stylefiles): Stylefiles for Narok Water, Kenya
- [WASAC/mapbox-stylefiles](https://github.com/WASAC/mapbox-stylefiles): Stylefiles for WASAC, Rwanda.

Those stylefiles are licenced under `C0-1.0 License`. However, we are using some icons of Mapbox Studio. So those icons which are from Mapbox, the license also belong them.



---
## Contributions

This vectortiles toolkit was developed and is maintained by Jin IGARASHI(see [portfolio](https://water-gis.com) if you are fascinated by more details about me). If you have any feedbacks, please let me know through Github's issues or pull request. Also, if you like my GIS works for water services providers in Africa, you can make donation through [Github Sponsor](https://github.com/sponsors/JinIgarashi).

---
`Copyright © 2020 Jin IGARASHI`
