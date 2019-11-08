# Commercial Clusters in Bengaluru City
## Geo-spatial Analysis of Data from Open Street Maps(OSM)

### **Aim:** Identify commercial centers using Points of Interest (POI) data  
There's a lot of open data available about the demographics and geography of the planet. But this information is not necessarily supervised in any particular structure from which insights can be drawn.  This task requires you to create clusters of distinct commercial centers or markets using points of interest data of a city (the city could be yours). Points of interest (POI) data provides location information of different places along with their defining tags like school, type of outlets, type of building, etc.  POI data refers to the coordinates of any physical entity with a tag describing its type like commercial buildings, schools, hospitals, restaurants, etc. 

**Objective:**  
* Get Points of Interest from open data sources like open street maps (OSM). 
* Understand how spatial location data works Understand spatial vector data types and how to manipulate it using your language of choice.
* Understand necessary GIS concepts like projections, spatial clustering, etc. 
* Figure out a way of clustering these points into commercial centers/markets. 
* You can use standard size polygons also to cluster the points. 
* Find and label the most significant clusters, statistically and intuitively.  
* Visualize the resultant commercial centres/markets.   

**Data Source:**  
POI (OSM) data- https://www.openstreetmap.org/ You can use overpy (a python frontend for overpass API of OSM) to get OSM data for the desired city.  (Tip: you can use overpass-turbo to frame queries)

## Files Description:
**Data Extraction:** *data_collection.ipynb*

**Output file:** *bengaluru_geo_data.csv* (Extracted Data of Bengaluru city)


**Data Analysis & Clustering:** *bengaluru_commercial_clusters.ipynb* (requires *bengaluru_geo_data.csv*)

**Output files:** 
* **ESRI Shapefiles:** *(bengaluru_commercial_clusters.shp, .shx, .prj, .cpg, .dbf)*
* **Cluster Dataframes:** *(bng_category_cluster.csv, commercial_cluster.csv)*

**Cluster Visualization:** *visualize_commercial_clusters.ipynb* (requires *bengaluru_commercial_clusters.shp, commercial_cluster.csv*)

## Requirements
Python >=3.7 (It's highly recommended to use the latest Anaconda Distribution)
Jupyter Notebook/Lab

**Libraries Used:**
* numpy
* pandas
* matplotlib
* geopandas (for geo-spatial analysis)
* overpy (python client for OverpassAPI)
* folium (for visualizations)
* shapely (for geo-spatial analysis)
* sklearn
* scipy
* hdbscan (for HDBSCAN clustering)
* descartes (for Polygon Patch )
<hr>
<h6 align='center'>Copyright (c) 2019 Albert Abraham </h6>
