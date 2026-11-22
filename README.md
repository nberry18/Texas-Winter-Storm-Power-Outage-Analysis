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
The SST data was originally generated from NOAA’s 5km Daily Global Satellite Sea Surface Temperature Anomaly v3.1. The datasets used in this analysis was obtained from a downloadable data folder provided through the Environmental Data Science 223 course at the University of California of Santa Barbara website by Annie Adams: https://eds-223-geospatial.github.io/assignments/HW3.html. 

Bathymetry dataset characterizes the depth of the ocean from the General Bathymetric Chart of the Oceans (GEBCO). This dataset was obtained from a downloadable data folder provided through the Environmental Data Science 223 course at the University of California of Santa Barbara website by Annie Adams: https://eds-223-geospatial.github.io/assignments/HW3.html. 

The Exclusive Economic Zones dataset is spatial dataset used to define the maritime boundaries using Exclusive Economic Zones off of the west coast of US from Marineregions.org. The Crashes data comes from the Statewide Integrated Traffice Records System (SWITRS) database collects and processes data gathered from a collision scenes. This dataset used in this analysis was obtained from a downloadable data folder provided through the Environmental Data Science 223 course at the University of California of Santa Barbara website by Annie Adams: https://eds-223-geospatial.github.io/assignments/HW3.html. 

## Author
Nina Berry: https://github.com/nberry18 

## References
- Average annual sea surface temperature (SST) from the years 2008 to 2012: average annual dataset: https://coralreefwatch.noaa.gov/product/5km/index_5km_ssta.php
- Ocean depth dataset: https://www.gebco.net/data_and_products/gridded_bathymetry_data/#area
- Exclusive Econonic Zones dataset: https://www.marineregions.org/eez.php
- 223 Homework 3 assignment description: https://eds-223-geospatial.github.io/assignments/HW3.html
