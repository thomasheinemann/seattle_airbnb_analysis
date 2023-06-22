# Airbnb Seattle analysis


### Summary

This project covers an analysis of data from 3818 Airbnb accommodations in Seattle and was triggered by the udacity "data-scientist-nanodegree" program (see https://www.udacity.com/).
Referring to these, accomodation data on actual price and availability over a one year period (starting from January 2016) as well as data on client reviews covering 3191 of our accommodations (between June 2009 and Jan. 2016) are taken into account. 
In total, this analysis deals with three business questions being discussed sequentially.



### Motivation

This investigation is part of a crisp-dm approach dealing with Seattle Airbnb data and is inspired by Josh Bernard who is a mentor in the prior-mentioned udacity program.
Given a rough idea about the data, I started asking business questions that were iteratively changed or specified. Finally, an answer to each business question is developed forming the base of a blog post.

### Data sources: 

survey data
- https://www.kaggle.com/datasets/airbnb/seattle

geographical data:
- https://data-seattlecitygis.opendata.arcgis.com/datasets/city-clerk-neighborhoods/explore?location=47.614536%2C-122.336950%2C12.4A

### Install/run instructions:
1. Install python >= 3.11 and the packages denoted in requirements_working_configuration.txt preferably in a virtual environment as exemplarily shown for the windows command prompt:
```
      projectfolder:> python -m venv .venv
      projectfolder:> cd .venv\Scripts
      projectfolder\.venv\Scripts> .\activate.bat
      projectfolder\.venv\Scripts> cd ..\..
      projectfolder:> python -m pip install -r requirements_working_configuration.txt
```
      Within your project folder "projectfolder" use the "python" command as long as the virtual environment is activated
      (if not working with/on the project, the virtual environment should be deactivated by executing projectfolder\.venv\Scripts\deactivate.bat).

      Important note: If you are using requirements.txt (no package versions provided) instead of requirements_working_configuration.txt, make shure to install ipykernel before (python -m pip install ipykernel). The order seems imnportant.

2. Download the Airbnb survey data from the link provided above (subscription required) and extract the three csv files into the "data" folder. The geographical data is downloaded automatically within the main jupyter file "analysis.ipynb".

3. In the programming IDE select .venv\Scripts\python.exe as Kernel.

4. Run all code blocks in "analysis.ipynb"

### Files in the repository
```
analysis.ipynb # main jupyter file
data           # contains files covering ETL pipeline
|- calendar.csv            # data about each Airbnb listing's price and availability                                 (has to be downloaded manually)
|- reviews.csv             # data about reviews from Airbnb customers covering a time interval between 2009 and 2016 (has to be downloaded manually)
|- listings.csv            # data about Airbnb listings in seattle covering id, host name, list price, ...           (has to be downloaded manually)
|- City_Clerk_Neighborhoods.cpg # neighbourhood shape data (will be downloaded automatically)
|- City_Clerk_Neighborhoods.dbf # neighbourhood shape data (will be downloaded automatically)
|- City_Clerk_Neighborhoods.prj # neighbourhood shape data (will be downloaded automatically)
|- City_Clerk_Neighborhoods.shp # neighbourhood shape data (will be downloaded automatically)
|- City_Clerk_Neighborhoods.shx # neighbourhood shape data (will be downloaded automatically)
graphics
|- airbnb_seattle_gender_ratio.png   # graph visualizing female reviewer gender ratio depending on the host's gender and review score
|- airbnb_seattle_influence_of_host_response_on_rating.png  # diagrams visualizing influence of host response on review scores rating with histograms
|- airbnb_seattle_price_fluctuation.png  # image visualizing Seattle's airbnb locations and their price fluctuation
|- airbnb_seattle_prices_per_neighbourhood_listing_price_desc.png    # table providing information about neighbourhoods whose Airbnb listings possess high listing prices
|- airbnb_seattle_prices_per_neighbourhood_price_deviation_desc.png  # table providing information about neighbourhoods whose Airbnb listings possess high deviations from their listing prices
README.md
requirements.txt                       # list of required packages
requirements_working_configuration.txt # packages covering a working configuration

```
