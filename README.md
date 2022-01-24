# JS-Maps-Training
A self training for checking how much I learned from onboarding course.
Since I am new to JavaScript, so I chose to make a JS based demo.
It's a map to show Japan covid-19 quasi-emergency prefectures.

> refered :https://docs.mapbox.com/help/tutorials/choropleth-studio-gl-pt-1/
## What I did

### 1.Download Dataset
Download Japan prefectures geojson data from (here)[https://github.com/dataofjapan/land/blob/master/japan.geojson]

* Tried the (carto)[https://tmfraser65.carto.com/tables/japan_prefectures/public/map] but somehow invalid errors happened when upload

### 2.Upload
The geojson file was too big(18Mb) to do it on Studio dataset, so made it to a tileset directly.

### 3.Use expression
* Use `Sytle across data range` or `Style with data conditions` also works but I tried API level this time.

* Found (this)[https://github.com/mapbox/mapbox-gl-js/issues/9862], said `setPaintProperty` couldn't re-render the layer. But I tried and looks fine.

* Better use csv or json to read date dynamically, but CORS problem happened, will be a todo
