# Project McNulty: Predicting Car Accident Injuries in New York State 

This project is a classification based modeling project to predict whether or not an injury will occur from a car crash. The data used is a list of vehicle accidents that occurred in New York State from 2014-2016. The data are sourced from [Kaggle](https://www.kaggle.com/new-york-state/nys-motor-vehicle-crashes-and-insurance-reduction) (motor-vehicle-crashes-case-information-three-year-window.csv specifically) 

## Files
Below you can find the purpose for each notebook in this repo:

### Danielo_McNulty_Presentation.pdf
Formal project slide deck

### Cleaning & Creating Final Dataframe.ipynb
Used to process the data to create the final DataFrame that will be used for modeling. Steps include:
* Mapping variables to groups and numerical values
* Dummifying categorical variables
* Joining data set with weather data
* Filling in NaNs using mean and mode by county 
* Feature Text Extraction

### Modeling Notbook.ipynb
Used to apply various classifcation models to the cleaned data set. Steps include:
* Splitting the data into training, validation and testing sets
* Apply Logistic Regression, Decision Tree, Random Forest, and Boosted Trees algos to the data set
* Plotting Confusion Matrices and scoring for model comparison

### Weather_data_scraper.ipynb
Used to scrape weather data for each of the counties. This script was borrowed and modified for the purposes of this project: Steps include:
* Extracting daily weather data from [TimeandDate.com](https://www.timeanddate.com/) for each month in the 2014-2016 timespan.
* Combining smaller dataframes 

### CombineWeatherFiles.ipynb
Used to combine the individual weather files for each county. Steps include:
* Getting a list of local pkl files
* Concatenating relevant files

## Extras
### Tableau EDA Dashboard: [HERE](https://public.tableau.com/profile/danielo.bennett#!/vizhome/NYS-Car_Accident_Dashboard/Dashboard2?publish=yes)
### Blog Post: Coming Soon!

