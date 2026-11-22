# EDS223 HW3: Houston, Texas Winter Storm Power Outage Analysis (February 2021)
Mapping Power Outages and Community Impacts in Houston, Texas

<img width="1600" height="900" alt="houston snow" src="https://github.com/user-attachments/assets/287e460e-01c9-4182-a6bd-605b9042eca2" />

## Purpose
This repository analyzes areas of Houston that experienced power outages during the February 2021 storms. This analysis removed highway buffers of 200 meters because outages near major roadways were not representative of residential power outages. The blackout raster was then filtered to identify areas where homes experienced a loss of power across the city. While this analysis identifies the spatial distribution of power outages, it does not examine the environmental justice implications of these disruptions. Future analysis should investigate whether the frequency and duration of outages differed across neighborhoods and whether vulnerable communities experienced disproportionate impacts. 

## Overview
Highlights:
- power_outage_analysis.qmd: highlights the spatial analysis of the 2021 storm in Houston, Texas that caused power outages across the city. This analysis used the stars package to load and run the data.
- Data folder: houses the VNP46A1 tif files(spatial maps of the power outages in Houston on 2/07/2021 and 2/16/2021),gis_osm_buildings_a_free_1.gpkg (types of building in Houston), and gis_osm_roads_free_1.gpkg (types of roads in Houston).

```{r}
Texas-Winter-Storm-Power-Outage-Analysis 
└───README.md
└─── power_outage_analysis.pdf   
└─── power_outage_analysis.qmd 
└───.gitignore
    └───data
        └───gis_osm_buildings_a_free_1.gpkg
        └───gis_osm_roads_free_1.gpkg
        └───VNP46A1
            └───VIIRS data files
```

## Data Access
The NASA VIIRS data (night lights) uses the NASA’s Worldview to explore the data around the day of the storm. This data included 2021-02-07 and 2021-02-16 since it provides two clear, contrasting images to visualize the extent of the power outage in Texas. The datasets used in this analysis was obtained from a downloadable data folder provided through the Environmental Data Science 223 course at the University of California of Santa Barbara website by Annie Adams: https://eds-223-geospatial.github.io/assignments/HW4.html. 

The Open Street Map dataset is shapefile of all highways in Texas in a prepared Geopackage (.gpkg file) containing just the subset of roads that intersect the Houston metropolitan area. The buildings Geopackage (.gpkg file) dataset was also collected and published through OSM. This dataset was obtained from a downloadable data folder provided through the Environmental Data Science 223 course at the University of California of Santa Barbara website by Annie Adams: https://eds-223-geospatial.github.io/assignments/HW3.html. 

## Author
Nina Berry: https://github.com/nberry18 

## References
- The data can be accessed at: https://drive.google.com/file/d/1bTk62xwOzBqWmmT791SbYbHxnCdjmBtw/view
- The data must be downloaded and unzipped to be used.
- The nighttime lights is sourced from NASA’s Worldview VIIRS data. VIIRS data is distributed by NASA’s Level-1 and Atmospheric Archive & Distribution System Distributed Active Archive Center (LAADS DAAC). That data can be accessed here: https://ladsweb.modaps.eosdis.nasa.gov/
- The roads and highways data is sourced from OpenStreetMap (OSM) and can be accessed here: https://planet.openstreetmap.org/
- The buildings and houses data is sourced from OpenStreetMap (OSM) and can be accessed here: https://planet.openstreetmap.org/
- 223 Homework 3 assignment description: https://eds-223-geospatial.github.io/assignments/HW3.html
