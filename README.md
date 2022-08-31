# Mapping_Earthquakes
The following is a visualization of global geographic earthquake data using Leaflet.js API, JavaScript, D3, and MapBox.

### Overview
This project was created to help our client create a dynamic map that illustrates multiple layer views and  filters that show (1) tectonic plate location, (2) global earthquake activity in the last seven days, as well as (3) earthquake data greater than 4.5, each of which can be selected by the user.

### Method
To create this dynamic map, we prepared an index.html file, a .js file that constructed the map using an API Key from mapbox.com, and several d3.json(). The complete build was segmented as follows:

### 1: Add Tectonic Plate Data. 

The earthquake data for the last seven days was taken from the earthquake.usgs.gov website https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_week.geojson The data was added to our d3.json() function to create the "Earthquakes" layer of our map.

The tectonic plate data was retrieved from the raw json file stored here: https://raw.githubusercontent.com/fraxen/tectonicplates/master/GeoJSON/PB2002_boundaries.json This url was added to our d3.json() to create our "Tectonic Plate" layer for the map.

We also created two different map-views using styline features from mapbox.com.

<img width="632" alt="Challenge_deliverable1" src="https://user-images.githubusercontent.com/104729703/187599151-3c514559-49dc-4fd5-9884-1973a794a5b1.png">

### 2: Add Major Earthquake Data

We then added another layer to our map that shows all major earthquake data ("Major Earthquakes"). This data was sourced from: https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/4.5_week.geojson A seperate coloring system was added to the markers for these earthquakes so that they could be easily discerned from other earthquakes by the user using the map layer selection menu.

<img width="626" alt="Challenge_deliverable2" src="https://user-images.githubusercontent.com/104729703/187599167-40d0f482-62bc-432f-9512-76a276dea778.png">

### 3: Add an Additional Map

Upon completing these layers, we added a third layer view to our map from mapbox.com that presents the data with a "dark" view.

<img width="626" alt="Challenge_deliverable3" src="https://user-images.githubusercontent.com/104729703/187599180-0f58ae0c-02f4-4008-990c-ae1420447694.png">
