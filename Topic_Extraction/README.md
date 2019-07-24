# Public and media perceptions of LinkNYC over the years of operation
## Description: As news cover both day-to-day city life and opinions of journalists, we believe that our textual analysis sheds a light on how both public and media perceptions of LinkNYC have changed over the years.

## Table of Contents
1. [Introduction](README.md#Problem)
1. [Folder Structure](README.md#Folder_Structure)
1. [Notes](README.md#Notes)
1. [Libraries Used](README.md#Libraries_Used)
1. [Data Sources](README.md#Data_Sources)
1. [Instructions](README.md#Instructions)

## Folder Structure
```
├── Topic_Extraction
  └── Data
  └── Src
      └── Related_article.ipynb
  └── README.md
```
## Notes
Related_article.ipynb - performs scraping of web articles related to Intersection Co. It also performs Topic modeling with LDA and generates output as well as word cloud.

### Libraries Used
```
import pandas as pd
import requests
import urllib.request
import time
from urllib.request import Request
from bs4 import BeautifulSoup
import re
import nltk
import string
from nltk.corpus import stopwords
from nltk.stem import WordNetLemmatizer
import gensim
import pyLDAvis.gensim
from gensim.models import LdaModel
from gensim.corpora import Dictionary
from nltk.tokenize import word_tokenize
from openpyxl import load_workbook
import os 
```
Installation instructions:
Packages can be simply installed through `pip install <package-name>` or `conda install <package-name>`.

### Data Sources
- Intersection Co
  - List of articles related to Intersection Co

### Output
- LDA Results
- LDA Word Cloud

## Instructions
The program is a jupyter notebook. If requirements for your system are all met, you can simply open the jupyter notebook and run it sequentially, run all cells is not generally reccomended.  