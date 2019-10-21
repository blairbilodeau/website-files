+++
type= "project"

# Project title.
title = "An analysis of spatial crime data in Chicago"

# Date this page was created.
date = 2018-12-19

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["B.L. Bilodeau"]

# Abstract.
abstract = ""

# Project summary to display on homepage.
summary = ""

# Digital Object Identifier (DOI)
doi = ""

# Tags (optional).
#   Set `tags = []` for no tags, or use the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = []

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["deep-learning"]` references 
#   `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects = []

# Optional external URL for project (replaces project detail page).
external_link = ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references 
#   `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides = ""

# Links (optional).
url_preprint = ""
url_pdf = "project/chicago/report.pdf"
url_slides = ""
url_video = ""
url_code = "https://github.com/blairbilodeau/crimes_in_chicago"

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
# links = [{icon_pack = "fab", icon="twitter", name="Follow", url = "https://twitter.com/georgecushen"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  # caption = "Photo by rawpixel on Unsplash"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  # focal_point = "Smart"
+++

# Introduction

This work is adapted from my final project for STA2101 (Applied Statistics I) taken with Prof. Jerry Brunner. All the code and data is available on my Github.

For this project I chose the option of analyzing some interesting data with Python. Using 3 datasets available from Kaggle, I investigated crime in Chicago from 2012 to 2016. The main goal of this is to explore data analysis in Python, specifically spatial plotting and multinomial logistic regression for determining relationships between crimes and the explanatory variables. Some questions I address are where crime occurs, what type of crime occurs, how crime in the area influences school quality, and how police station locations are related to crime hotspots.

The primary dataset used is [crimes](https://www.kaggle.com/currie32/crimes-in-chicago#Chicago_Crimes_2012_to_2017.csv), which contains all reported incidents of crime in Chicago from 2012 to 2016. To supplement this, there is schools, which contains the progress report card of each public Chicago high school from the 2013-14 school year, and [police](https://www.kaggle.com/chicago/chicago-police-stations#police-stations.csv), which contains location info for all Chicago police stations. These datasets have many fields, so I will only mention the critical ones that are used in a model.
First, I import the libraries I will require.

```python
import numpy as np 
import pandas as pd 
import matplotlib.pyplot as plt
import matplotlib.patches as mpatches
import statsmodels.api as sm
from scipy.stats import chi2
from scipy.stats import norm
from scipy.special import logsumexp
from colour import Color
from random import choice
```

# Crime Severity

The initial crimes file contains 1,456,714 rows, where each row corresponds to a crime being reported, but I removed 37,174 of these for missing location data. I also excluded crimes from 2017 since there were only 30, so it was logical to just consider years which were fully reported. The field crimes[Primary Type] details the main reason for a crime being reported, and I cleaned this up by removing some white space and grouping types such as “NARCOTICS” and “OTHER NARCOTIC VIOLATION”. I split crimes[Date] into three fields for day, month, and year, and then dropped some redundant fields. A field that may have been useful is crimes[Description], which contains a sentence describing the crime in more depth, but I decided there was too much variability in them to be practical for this analysis.

```python
## Crimes Data Exploration

# We have 1 456 714 rows total
crimes = crimes[pd.notnull(crimes['X Coordinate'])] # 37 083 have NaN for location
crimes = crimes[crimes['X Coordinate'] > 0] # 77 have 0 for location
crimes = crimes[pd.notnull(crimes.Ward)] # 14 have NaN for ward
crimes = crimes[pd.notnull(crimes.District)] # 1 have NaN for district
crimes = crimes[pd.notnull(crimes['Community Area'])] # 22 have NaN for district
crimes = crimes[crimes.Year < 2017] # Only 30 crimes in 2017

# Clean up primary types
crimes = crimes.replace({'Primary Type':['NON - CRIMINAL', 'NON-CRIMINAL (SUBJECT SPECIFIED)']}, {'Primary Type':'NON-CRIMINAL'})
crimes = crimes.replace({'Primary Type':'OTHER NARCOTIC VIOLATION'}, {'Primary Type':'NARCOTICS'})
crimes = crimes.replace({'Primary Type':'CONCEALED CARRY LICENSE VIOLATION'}, {'Primary Type':'WEAPONS VIOLATION'})

# Time of event fields
crimes['Month'] = [int(date[0:2]) for date in crimes.Date]
crimes['Day'] = [int(date[3:5]) for date in crimes.Date]
crimes['Year'] = [int(date[6:10]) for date in crimes.Date] 

# Convert boolean to integer
crimes.Arrest = crimes.Arrest.astype(int)
crimes.Domestic = crimes.Domestic.astype(int)

# Lots of columns we don't care about
crimes.drop(['Unnamed: 0', 'Date', 'ID', 'Case Number', 'IUCR', 'Description', 'Location', 
	'Location Description', 'Updated On', 'Block', 'FBI Code'], axis=1, inplace=True)
```
