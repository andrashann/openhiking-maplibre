# Unofficial OpenHiking style for MapLibre: online demo

An unofficial hiking map in the look of the [OpenHiking](https://github.com/openhiking/openhiking-mapsforge) mapsforge map, as a static page, using vector tiles from [OpenFreeMap](https://openfreemap.org/). It is an independent port and is not made or endorsed by the OpenHiking project.

## What it shows

- The base map: [OpenFreeMap](https://openfreemap.org/) vector tiles, drawn with `openhiking.json` or, in dark mode, `openhiking-dark.json`.
- Hillshading and contour lines, computed in the browser from [Mapterhorn](https://mapterhorn.com/) terrain tiles.
- Marked hiking, cycling, and mountain bike routes, as overlays from [Waymarked Trails](https://waymarkedtrails.org/), each with a checkbox.

Dark mode is an addition of this project and not part of OpenHiking (see Credits). Its checkbox follows the system setting until it is used; the choice and the map position are kept in the URL, so a link reproduces the view.

OpenFreeMap's tiles do not contain everything the OpenHiking map shows. Springs, caves, lookout towers, the distinction between path types, and the trails themselves are missing from the base map, which is why the routes come from an overlay.

## Files

| File | Content |
| --- | --- |
| `index.html` | The page. |
| `openhiking.json`, `openhiking-dark.json` | The MapLibre styles. |
| `sprite/` | The icons of the styles. |
| `LICENSE` | GPL-3.0, the license of the OpenHiking theme and icons, which the styles and the sprite derive from. |
| `.nojekyll` | Tells GitHub Pages to serve the files unprocessed. |

## Credits

- Map data: © [OpenStreetMap](https://www.openstreetmap.org/copyright) contributors (ODbL).
- Vector tiles: served by [OpenFreeMap](https://openfreemap.org/), in the tile schema of [OpenMapTiles](https://www.openmaptiles.org/) (© OpenMapTiles, CC BY).
- Style and icons: after [OpenHiking](https://github.com/openhiking/openhiking-mapsforge) (GPL-3.0-only). The light style is a port of its mapsforge theme. The dark style is not by OpenHiking, which has no night theme: it is this project's own palette on the same layers, keeping the color roles of the original (green forest, blue water, the road and trail colors).
- Elevation: [Mapterhorn](https://mapterhorn.com/attribution) and its sources.
- Routes: [Waymarked Trails](https://waymarkedtrails.org/) (CC BY-SA), from OpenStreetMap data.
- Rendering: [MapLibre GL JS](https://maplibre.org/) and maplibre-contour.

