## Web Map Service \(WMS\)

A standard protocol developed by the [Open Geospatial Consortium](https://en.wikipedia.org/wiki/Open_Geospatial_Consortium) in 1999 for serving [georeferenced](https://en.wikipedia.org/wiki/Georeference) map images over the Internet.

---

Request:

* GetMap – returns a map image. 
  * width and height of the map
  * coordinate reference system
  * rendering style
  * image format

e.g. [google map api](https://developers.google.com/maps/documentation/javascript/tutorial)

```js
map = new google.maps.Map(document.getElementById('map'), {
  center: {lat: -34.397, lng: 150.644},
  zoom: 8
});
```

---

This service is available from almost all map provider:

* ArcGIS Server
* Google Map
* GeoWebPublisher from Bentley
* Infrastructure Map Server from Autodesk
* osgEarth
* Matlat and Mapping Toolbox
* OpenLayers
* Leaflet.js



