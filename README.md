# Commercial Centers using POI data

- Identify commercial centers using Points of Interest (POI) data  

Create clusters of distinct commercial centers or markets using points of interest data of a city.


## Requirements:

- Python3
- Jupyter Notebook

**Libraries**

- Overpy
- GeoPandas
- Folium
- HDBScan
- Scipy
- Shapely

## RUN:

- [Commercial_Clusters_using_POI.ipynb]('Commercial_Clusters_using_POI.ipynb')

## Methodolgy:

### Collecting of Data

POI data is collected from an open source OpenStreetMap using OverpassTurbo. Alterntively, This can also be done using "Overpy" library.

### Clustering

For clustering, HDBScan is used which extends DBScan clustering algorithm and converts it into a hierarchical clustering algorithm. Since, we are working on GIS point cluster density based clustering algorithm seems to be more suitable than distance based.

### Most Significant CLuster

The most significant cluster is identified using statistics to find out the cluster with most number of amenities and also intuitively selecting one with variety of commercial amenities.
