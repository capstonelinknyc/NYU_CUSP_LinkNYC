# Exploratory Data Analysis
## Description: This repository contains file related to the exploratory analysis performed by the group

## Table of Contents
1. [Introduction](README.md#Problem)
2. [Folder Structure](README.md#Folder_Structure)
3. [Notes](README.md#Notes)
4. [Libraries Used](README.md#Libraries_Used)
5. [Data Sources](README.md#Data_Sources)
6. [Instructions](README.md#Instructions)

## Folder Structure
```
├── EDA
  └── Data
  └── Src
      └── census_age.ipynb
      └── census_and_linknyc_usage_data_merging_and_spatial_joins.ipynb
      └── correlation_demographics.ipynb
      └── Merge_Installed_and_Proposed_links.ipynb
      └── merger_file.ipynb
  └── README.md
```
## Notes
census_age.ipynb - Generate Age Demographic statistics and visualizations  
census_and_linknyc_usage_data_merging_and_spatial_joins.ipynb - Prepares data for Tableau maps and other visualizations  
correlation_demographics.ipynb - Checks correlation of LinkNYC EBT calls and income demographics  
Merge_Installed_and_Proposed_links.ipynb - Prepares data join together LinkNYC proposed kiosk locations and current LinkNYC kiosk locations  
merger_file.ipynb - Generate Income correlation heatmap-matrix and Visualizations  

### Libraries Used
```
import pandas as pd
import geopandas as gpd
import numpy as np
import xlrd
import shapely
import sys
from fiona.crs import from_epsg
import os
import math
import seaborn as sns
from sklearn.preprocessing import LabelEncoder
```
Installation instructions:
To install Geopandas, please refer to the following link [here](http://geopandas.org/install.html "Geopandas Installation Guide").  
Fiona and Shapely is typically installed during Geopandas installation.  
Other packages can be simply installed through `pip install <package-name>` or `conda install <package-name>`.

### Data Sources
- American Community Survey
  - Income
  - Age
- Intersection Co
  - LinkNYC Monthly usage
  - LinkNYC - Electronic Benefits Transfer
- NYC Open Data
  - Boundaries - Census Tracts
  - LinkNYC Kiosk Locations
  - LinkNYC Proposed Sites Permits
- Policymap
  - Supplemental Nutrition Assistance Program (SNAP)
  - Broadband Access in NYC 

### Output
- EDA results

## Instructions
The program is a jupyter notebook. If requirements for your system are all met, you can simply open the jupyter notebook and run it sequentially, run all cells is not generally reccomended.  