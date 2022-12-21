# 3D Scene Overview

This is a modification of the Overview Map sample on ArcGIS Developers: [ArcGIS Maps SDK for JavaScript
Sample Code | Overview Map](https://developers.arcgis.com/javascript/latest/sample-code/overview-map/)

## Configure URL parameters

The default app uses a webmap with the Equal Earth projection in the main view and uses the Light Gray Basemap for the overview globe. [Example](https://davidasbury.github.io/scene-overview-map)

### To change the main map use this convention:

``<base URL>?webmap=<webmap ID>`` 

where ``<webmap ID>`` is any ArcGIS Online webmap item. 

Example: [https://davidasbury.github.io/scene-overview-map/?webmap=22d1524dde5f4e5b9670545f5b853517](https://davidasbury.github.io/scene-overview-map/?webmap=22d1524dde5f4e5b9670545f5b853517)

The main map can be in **any** projection.

### To change the overview map:

``<base URL>?webmap=<webmap ID>&overview=<webmap ID2>``

where ``<webmap ID2>`` is any ArcGIS Online webmap in WGS84 or Web Mercator projection. This is a requirement of the [3D SceneViewer](https://developers.arcgis.com/javascript/latest/api-reference/esri-views-SceneView.html#spatialReference).

Example: [https://davidasbury.github.io/scene-overview-map/?webmap=8dda0e7b5e2d4fafa80132d59122268c&overview=67ab7f7c535c4687b6518e6d2343e8a2](https://davidasbury.github.io/scene-overview-map/?webmap=8dda0e7b5e2d4fafa80132d59122268c&overview=67ab7f7c535c4687b6518e6d2343e8a2)
