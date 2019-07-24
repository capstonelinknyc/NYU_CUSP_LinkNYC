# Does LinkNYC affects 311 requests type and total counts? 
## Description: This repository contains related to generation of analysis and visualizations related to 311 noise complaints.

## Table of Contents
1. [Introduction](README.md#Problem)
1. [Folder Structure](README.md#Folder_Structure)
1. [Notes](README.md#Notes)
1. [Libraries Used](README.md#Libraries_Used)
1. [Data Sources](README.md#Data_Sources)
1. [Instructions](README.md#Instructions)

## Folder Structure
```
├── 311_Calls
  └── Data
  └── Src
        └── 311_type_changes.ipynb
        └── LinkNYC_Usage_Correlation_Analysis.ipynb
        └── LinkNYC_with_City_Services.ipynb
  └── README.md
```
## Notes
311_type_changes.ipynb - Check on how 311 related complaints changed with the introduction of LinkNYC Kiosk based on analysis of keywords  
LinkNYC_Usage_Correlation_Analysis.ipynb - Check on correlation of 311 and broadband access with LinkNYC usage  
LinkNYC_with_City_Services.ipynb - Further analysis on how 311 changed with the introduction of LinkNYC Kiosks, performed hypothesis testing  

### Libraries Used
```
import numpy as np
import pandas as pd
import pylab as pl
import geopandas as gpd
import os
import datetime as dt
from matplotlib import gridspec
from fiona.crs import from_epsg
import shapely
from sodapy import Socrata
```
Installation instructions:
To install Geopandas, please refer to the following link [here](http://geopandas.org/install.html "Geopandas Installation Guide").  
Fiona and Shapely is typically installed during Geopandas installation.  
Packages can be simply installed through `pip install <package-name>` or `conda install <package-name>`.

### Data Source
- 311 Calls Data - Obtrained through SodaPy
- American Community Survey - Broadband access - Obtained through PolicyMap
- NYC Open Data
  - LinkNYC Kiosk Locations
  - LinkNYC Kiosk Permits
  - Spatial Data (shapefiles)
- Intersection Co
  - LinkNYC Kiosk data 

## Instructions
The program is a jupyter notebook. If requirements for your system are all met, you can simply open the jupyter notebook and run it sequentially.  