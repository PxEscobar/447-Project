# 447-Project
Covid Dashboard Web App for CMSC 447

I followed this tutorial - https://leafletjs.com/examples/choropleth/

Most of the changes here are inside home.html
Inside html files, anything inside of <script> tags is where you can use javascript
  
- In the header of base.html, leaflet.css and leaflet.js (map stuff) are included and extended to all html files
- In home.html
  
  - line 5 \<div id="map"> \</div> is where the map should show up on the page
       
  - lines 32 through ... 268,867 (LOL) is the map code
  
    - Map Stuff
      - map('map') links to the div (I think) 
      - titleLayer() is what builds the main layer of the map
      - getColor(), style(), highlightFeature(), resetHighlight(), zoomToFeature(), and onEachFeature()
        - these are used for specific features of the map
      - geoJson() is where where we pass a geoJson variable
        - ***the geojson variable*** contains data for the outline of each state county, as well as our data we want to pass to the map
      - control() creates a "control" variable, ours is called ***info***
        - all the code below control() is for the live pop up stuff you get when you hover over something
      
      
