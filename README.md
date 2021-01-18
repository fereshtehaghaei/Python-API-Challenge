# Python API - What's the Weather Like?

##### "What's the weather like as we approach the equator?"

Created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator, utilizing a [simple Python library](https://pypi.python.org/pypi/citipy) the [OpenWeatherMap API ](https://openweathermap.org/api) and create a representative model of weather across world cities.

To see my Python script, check jupyter notebook [here](https://github.com/fereshtehaghaei/Python-API-Challenge/blob/master/WeatherPy/WeatherPy.ipynb)



## Observation

- Southern Hemisphere climates tend to be slightly milder than those at similar latitudes in the Northern Hemisphere. This is because the Southern Hemisphere has significantly more ocean and much less land; water heats up and cools down more slowly than land.
- Highest temperature is found at 0 latitude and as the latitude increases or decreases, temperature drops. This happens as equatorial region receives sunlight straight with less or no angle due to curvature shape of earth.
- "Latitude doesn't have a strong influence on wind speed. The speed of the wind is controlled by the strength of the air pressure gradient, the stronger the pressure gradient the higher the wind speed. 



![](Images/equatorsign.png)



#  Part I - WeatherPy

------

- Created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator.


### Perform API Calls

- Performed a weather check on each city using a series of successive API calls.

### Print log of each city

- Included a print log of each city as it's being processed (with the city number and city name).

  



# Plotting the Data

- Used proper labeling of the plots using plot titles (including date of analysis) and axes labels.
- Saved the plotted figures as .pngs.

## Latitude vs. Temperature Plot 



![](Images/Lat_vs_Temp_Scatterplot.png)



## Latitude vs. Humidity Plot

![](Images/Lat_vs_Humid_Scatterplot.png)



## Latitude vs. Cloudiness Plot

![](Images/Lat_vs_Cloud_Scatterplot.png)

## Latitude vs. Wind Speed Plot

![](Images/Lat_vs_Wind_Scatterplot.png)



## Northern & Southern Hemisphere Data-Frame



#### Northern Hemisphere - Max Temp vs. Latitude Linear Regression

![](Images/Northern_Hem_Lat_vs_Temp_Scatterplot.png)



```
The r-value is: 0.8159776172443847
The correlation between Latitude and Max Temperature in Northern Hemisphere is -0.9
```



#### Southern Hemisphere - Max Temp vs. Latitude Linear Regression

![](Images/Southern_Hem_Lat_vs_Temp_Scatterplot.png)

```
The r-value is: 0.4866761323760189
The correlation between Latitude and Max Temperature in Southern Hemisphere is 0.7
```



#### Northern Hemisphere - Humidity (%) vs. Latitude Linear Regression

![](Images/Northern_Hem_Lat_vs_Humid_Scatterplot.png)

```
The r-value is: 0.0763245518304966
The correlation between Latitude and Humidity in Northern Hemisphere is 0.28
```



#### Southern Hemisphere - Humidity (%) vs. Latitude Linear Regression

![](Images/Southern_Hem_Lat_vs_Humid_Scatterplot.png)

```
The r-value is: 0.020275065972691547
The correlation between Latitude and Humidity in Southern Hemisphere is 0.14
```



#### Northern Hemisphere - Cloudiness (%) vs. Latitude Linear Regression

![](Images/Northern_Hem_Lat_vs_Cloud_Scatterplot.png)

```
The r-value is: 0.07149840247516427
The correlation between Latitude and Cloudiness in Northern Hemisphere is 0.27
```



#### Southern Hemisphere - Cloudiness (%) vs. Latitude Linear Regression

![](Images/Southern_Hem_Lat_vs_Cloud_Scatterplot.png)

```
The r-value is: 0.03918331683452775
The correlation between Latitude and Cloudiness in Southern Hemisphere is 0.2
```



#### Northern Hemisphere - Wind Speed (mph) vs. Latitude Linear Regression

![](Images/Northern_Hem_Lat_vs_WindSpeed_Scatterplot.png)

```
The r-value is: 0.005313203667376115
The correlation between Latitude and Wind Speed(mph) in Northern Hemisphere is 0.07
```



#### Southern Hemisphere - Wind Speed (mph) vs. Latitude Linear Regression

![](Images/Southern_Hem_Lat_vs_WindSpeed_Scatterplot.png)

```
The r-value is: 0.13204377443082696
The correlation between Latitude and Wind Speed(mph) in Southern Hemisphere is -0.36
```



# Part II - VacationPy

I used jupyter-gmaps and the Google Places API and used my skills in working with weather data to plan future vacations. 

### Plotting Heatmap

- Created a heat map that displays the humidity for every city from the part I of the project.

  ![](Images/Heat_Map.png)

- Narrow down the Data-Frame to find my ideal weather condition. For example:

  - A max temperature lower than 80(°F) degrees but higher than 70(°F). For this section, I used metric measurement so my max temp lower than 26.66(°C) but higher than 21.1(°C)

  - Wind speed less than 10 mph.

  - Zero cloudiness.

  - Drop any rows that don't contain all three conditions.

    

  ### Hotel Map

  ![](Images/hotel_map.png)

  

  ## To run the code:

  - Install citypy in your python environment (https://pypi.python.org/pypi/citipy)
  - Save OpenWeatherMap API Key (https://openweathermap.org/) as 'weather_api_key'
  - Google API Key (https://console.developers.google.com/getting-started) as 'g_key'
  - Create API Keys and store it in the 'api_keys.py' file before running the Jupyter notebooks.

  

  ### Copyright

  Fereshteh Aghaei © 2021. All Rights Reserved.