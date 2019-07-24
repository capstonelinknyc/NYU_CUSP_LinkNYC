# Patterns in EBT usage and households receiving SNAP benefits 
## Description: Intersection Co previously observed that LinkNYC kiosks are often used by people dependent on Supplemental Nutrition Assistance Program (SNAP) benefits, commonly known as food stamps.

## Table of Contents
1. [Introduction](README.md#Problem)
1. [Folder Structure](README.md#Folder_Structure)
1. [Notes](README.md#Notes)
1. [Instructions](README.md#Instructions)

## Folder Structure
```
├── EBT
  └── Data
  └── Src
      └── food_stamps_exploration_cleaned.ipynb
  └── README.md
```
## Notes
### Libraries Used
```
try:
    import urllib2 as urllib
except ImportError:
    import urllib.request as urllib
import requests 
import pandas as pd
from shapely.geometry import Point
import geopandas as gpd
from fiona.crs import from_epsg
import pylab as pl
import matplotlib.pyplot as plt
from sklearn.cluster import KMeans
```
Installation instructions:
To install Geopandas, please refer to the following link [here](http://geopandas.org/install.html "Geopandas Installation Guide").  
Fiona and Shapely is typically installed during Geopandas installation.  
Other packages can be simply installed through `pip install <package-name>` or `conda install <package-name>`.

### Data Sources
- [OpenNYC - Boroughs Boundaries](https://data.cityofnewyork.us/Housing-Development/Public-Use-Microdata-Areas-PUMA-/cwiz-gcty)
- Intersection Co
  - LinkNYC Monthly usage
  - LinkNYC - Electronic Benefits Transfer

### Output
- EDA results

## Instructions
The program is a jupyter notebook. If requirements for your system are all met, you can simply open the jupyter notebook and run it sequentially, run all cells is not generally reccomended.  