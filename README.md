# Airbnb Seattle analysis


### Summary

This project covers an analysis on data from 3818 Airbnb-listings in Seattle and was triggered by the udacity "data-scientist-nanodegree" program (see https://www.udacity.com/).
Referring to these listings data on actual price and availability over a one year period (starting from the 4th of January 2016) as well as data on client reviews covering 3585 properties (between Sept. 2009 and Sept. 2016) are taken into account as well. Corresponding data sources are referred in markdowns in the jupyter file.
In total, this analysis deals with three business questions being discussed sequentially.



### Motivation

This investigation is a part of a crisp-dm approach about Seattle Airbnb data and is inspired by Josh Bernard who is a mentor in the udacity "data-scientist-nanodegree" program (see https://www.udacity.com/).
Given a rough idea about the data I started asking business questions which
were iteratively changed or precised during the steps above. Finally an answer to each business question is developed forming the base of a blog post.

### Data source: 

survey data
- https://www.kaggle.com/datasets/airbnb/seattle

geographical data:
- https://data-seattlecitygis.opendata.arcgis.com/datasets/city-clerk-neighborhoods/explore?location=47.614536%2C-122.336950%2C12.40

### Install/run instructions:
0. Install the packages denoted in requirements_working_configuration.txt preferably in a virtual environment as exemplarily shown for the windows command prompt:
```
      projectfolder:> python -m venv venv
      projectfolder:> cd venv\Scripts
      projectfolder\venv\Scripts> .\activate.bat
      projectfolder\venv\Scripts> cd ..\..
      projectfolder:> python -m pip install -r requirements_working_configuration.txt
```
      Within your project folder "projectfolder" use the "python" command as long as the virtual environment is activated
      (if not working with/on the project, the virtual environment should be deactivated by executing projectfolder\venv\Scripts\deactivate.bat).

1. Run the following commands in the project's root directory to set up your database and model.

### Files in the repository
```
data           # contains files covering ETL pipeline
|- calendar.csv            # data about each airbnb-listing's price and availability
|- reviews.csv             # data about reviews from airbnb customers covering a time interval between 2009 and 2016
|- listings.csv            # data about airbnb-listings in seattle covering id, host name, list price, ...
README.md
requirements.txt                       # list of required packages
requirements_working_configuration.txt # packages covering working configuration
seattles_airbnb_price_fluctuation.png  # picture covering seattles airbnb price deviation from the list price
```
