# Forest Fires

![Wild-fires](https://user-images.githubusercontent.com/64386278/91287946-03111b80-e7ae-11ea-8ce6-736a38ea68b9.jpg)

 
  **Objective**
 
Forest fires help in the natural cycle of woods' growth and replenishment. They Clear dead trees, leaves, and competing vegetation from the forest floor, so new plants can grow. Remove weak or disease-ridden trees, leaving more space and nutrients for stronger trees.

But when fires burn too hot and uncontrollable or when they’re in the “wildland-urban interface” (the places where woodlands and homes or other developed areas meet), they can be damaging and life threatning.

In this kernel, our aim is to predict the burned area (area) of forest fires, in the northeast region of Portugal. Based on the the spatial, temporal, and weather variables where the fire is spotted.

This prediction can be used for calculating the forces sent to the incident and deciding the urgency of the situation.
 
 # About Data:
 
 * This dataset covers meteorological and spatiotemporal data for forest fires (between 2000 and 2003) in Portugal’s Montesinho Natural Park, with 13 attributes each for 517 such incidents. 
 
 * Our target attribute from these 13 is ‘area’ - total burned area in hectares (ha). 
 
 * The corresponding weather data is that which is registered by sensors when the fire was detected (or first broke out). We have: temp, RH (relative humidity), wind (speed), rain (accumulated precipitation over the last 30 minutes)
  
  * We also have DMC, DC, ISI and FFMC are components of the Canadian Forest Fire Weather Index (FWI) System, which measures the effects of fuel moisture and wind on fire behavior. These have been calculated using consecutive daily observations of temperature, relative humidity, wind speed, and 24-hour rainfall - i.e. these are time-lagged and not instantaneous values, unlike the four weather variables. Roughly, the higher these components, the more the expected severity of the fire.
  
* Spatiotemporal data includes the month and day of the week that the incident occurred, and X and Y co-ordinates of the incident with respect to the park. Smaller fires are much more frequent. This is the case in this dataset, as well as with incidences of wildfires around the world, making this a difficult regression problem

## Outline
    #  Load and describe data  
    #  Missing value treatment  
    #  Exploratory Data Analysis  
         - Univariate analysis  
         - Bivariate analysis with our target variable             
         - Multivariate analysis  
    #  Outlier treatment  
    #  Preparing the data for modelling  
    
 # Models:
  * Linear Regression
  * Bagging Regressor
  * Extra Trees Regressor
  * K-Nearest Neighbor
  * Decision Tree
  * Random Forest
  * Support Vector Machine
