## Web Map Tile Service \(WMTS\)



An open standard for geo-referenced map tiles over the internet.

The specification was developed and first published by the [Open Geospatial Consortium](https://en.wikipedia.org/wiki/Open_Geospatial_Consortium) in 2010.

![](/assets/earth_wmts_bingmap.jpg)

![](/assets/earth_WMTStilematrix_en.png)

---

#### Comparison

| WMS | WMTS |
| :--- | :--- |
| on-the-fly-rendering | pre-rendered tiles |
| Long response time: 1 or more CPU seconds \(for rendering\) | quick response: locate a file |
| not practical for massive parallel requests | directly use quad-tree |
| N/A | view-dependent optimization |
|  |  |

---

#### Request:

* layer
* level
* x \(column\)
* y \(row\)

Google tile example

```js
http://mt1.google.com/vt/lyrs=y&x=1325&y=3143&z=13
```

![](/assets/earth_lyrs=y&x=1325&y=3143&z=13.jpg)

---

#### Providers:

* google
* bing
* open street map
* carbon
* tencent
* 高德
* 天地图

Baidu does not follow WMTS standard.

Possible to use but the service is **commonly not commercialized**.

We are still looking for stable, fast, legitimated tile service. 

