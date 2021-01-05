---
title: "Assignment"
output: 
  html_document:
    keep_md: true 
---


## Date

5-Jan-2021

## Background

Create a web page using R Markdown that features a map created with Leaflet. 

Host your webpage on either GitHub Pages, RPubs, or NeoCities.


## Map Creation


```r
library(leaflet)
```

```
## Warning: package 'leaflet' was built under R version 4.0.3
```

```r
my_map <- leaflet() %>% addTiles() 
my_map <- my_map %>% addMarkers(lat=43.651070, lng= -79.347015, popup="Toronto")
my_map
```

<!--html_preserve--><div id="htmlwidget-f057e5950ce5c62b01b9" style="width:672px;height:480px;" class="leaflet html-widget"></div>
<script type="application/json" data-for="htmlwidget-f057e5950ce5c62b01b9">{"x":{"options":{"crs":{"crsClass":"L.CRS.EPSG3857","code":null,"proj4def":null,"projectedBounds":null,"options":{}}},"calls":[{"method":"addTiles","args":["//{s}.tile.openstreetmap.org/{z}/{x}/{y}.png",null,null,{"minZoom":0,"maxZoom":18,"tileSize":256,"subdomains":"abc","errorTileUrl":"","tms":false,"noWrap":false,"zoomOffset":0,"zoomReverse":false,"opacity":1,"zIndex":1,"detectRetina":false,"attribution":"&copy; <a href=\"http://openstreetmap.org\">OpenStreetMap<\/a> contributors, <a href=\"http://creativecommons.org/licenses/by-sa/2.0/\">CC-BY-SA<\/a>"}]},{"method":"addMarkers","args":[43.65107,-79.347015,null,null,null,{"interactive":true,"draggable":false,"keyboard":true,"title":"","alt":"","zIndexOffset":0,"opacity":1,"riseOnHover":false,"riseOffset":250},"Toronto",null,null,null,null,{"interactive":false,"permanent":false,"direction":"auto","opacity":1,"offset":[0,0],"textsize":"10px","textOnly":false,"className":"","sticky":true},null]}],"limits":{"lat":[43.65107,43.65107],"lng":[-79.347015,-79.347015]}},"evals":[],"jsHooks":[]}</script><!--/html_preserve-->
