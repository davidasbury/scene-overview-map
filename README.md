# 3D Scene Overview

This is a modification of the Overview Map sample on ArcGIS Developers: [ArcGIS Maps SDK for JavaScript
Sample Code | Overview Map](https://developers.arcgis.com/javascript/latest/sample-code/overview-map/)

## Configure URL parameters

The default app uses a webmap with the Equal Earth projection in the main view and uses the Light Gray Basemap for the overview globe.

### To change the main map use this convention:

``<base URL>?webmap=<webmap ID>`` 

where ``<webmap ID>`` is any ArcGIS Online webmap item.

The main map can be in **any** projection.

### To change the overview map:

``<base URL>?webmap=<webmap ID>&overview=<webmap ID2>``

where ``<webmap ID2>`` is any ArcGIS Online webmap in WGS84 or Web Mercator projection. This is a requirement of the [3D SceneViewer](https://developers.arcgis.com/javascript/latest/api-reference/esri-views-SceneView.html#spatialReference).
