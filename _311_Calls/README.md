# Does LinkNYC affects 311 requests type and total counts? 
## Description:

## Table of Contents
1. [Introduction](README.md#Problem)
1. [Folder Structure](README.md#Folder_Structure)
1. [Notes](README.md#Notes)
1. [Instructions](README.md#Instructions)

## Folder Structure
```
├── 311_Calls
  └── Data
  └── Src
  └── README.md
```
## Notes
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
To install Sodapy, please refer to the following link [here](https://github.com/xmunoz/sodapy "Sodapy Installation Guide").
All other packages can be installed using 


### Data Source
311 Calls Data - Obtrained through SodaPy
American Community Survey - 
LinkNYC Kiosk data - Provided by Intersection Co

### Output

## Instructions
The program is a jupyter notebook. If requirements for your system are all met, you can simply open the jupyter notebook and run it sequentially.  