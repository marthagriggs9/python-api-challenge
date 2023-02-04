# python-api-challenge
## Summary 


The following data was collected to visualize the weather of over 500 cities of varying distances from the equator. 
I used the citypy Python library and the OpenWeatherMap API to help create a representative model of weather across cities. A series of scatter plots were created to showcase the following relationships:
* Latitude vs. Temperature
* Latitude vs. Humidity
* Latitude vs. Cloudiness
* Latitude vs. Wind Speed

The data was split into Northern and Southern Hemisphere and linear regression models were added to the scatter plots to create a visual representation of any possible trends. 
After creating a DataFrame with the information gathered from the various cities (City, Country, Latitude, Longitude, Max Temp, Humidity, Cloudiness, Windspeed and Date collected), this information was used to help plan future vacations. 
Using Jupyter notebook, geoViews Python library and the Geoapify API map, visualizations were created to represent all cities from the DataFrame. 
The results were then narrowed down based on temperature and humidity preferences.
Hotels in each city that met the criteria were found and a new map was created that can be used to find this information. 

## Linear Relationship Findings:

* For the Northern Hemisphere, there is a strong negative correlation, meaning the further away from the equator (zero degrees latitude), the lower the temperature. This is generally expected when considering temperature and proximity to the equator. 
* For the Southern Hemisphere, the r-squared value of 0.1534371429008172 shows that there doesn't seem to be a correlation between latitude and maximum temperature. This could be due to the current season(spring) having a wider range of temperatures experienced by the given cities. It's also important to note that the Southern Hemisphere filtering only produced 184 data points compared to 389 data points returned for the Northern Hemisphere filter, so if the data sets had similar numbers to compare, we may see a stronger correlation between latitude and maximum temperature in the Southern Hemisphere as well. 
* Humidity is the measure of water vaopr in the air. For either hemisphere, there is a very weak correlation between latitude and humidity. Latitude does not seem to be a reliable way to predict humidity. Humidity may be better predicted by how far a place is from a large body of water, like an ocean, or compared to another factor like temperature or cloudiness. 
* When comparing latitude and percent cloudiness, there does not seem to be a correlation between the two factors for either hemisphere. For both hemispheres there are interstingly clusters of 100% cloudiness over various latitudes. 
* There is no strong relationship between latitude and wind speed (meters per second) for either hemisphere. Wind speed in the Northern Hemisphere clustered around 5 m/s across all latitudes in the data set (this would be around 11.18mph or lower). Most wind speeds for both hemispheres were below 10 m/s (below 22.37mph). 
* There was very detailed information that could be extracted from the OpenWeatherMap API, but the data collected represented just a snippet of time. A better determinant of predicting weather seems to be following weather data of a certain place over longer periods of time (much like local meterologists do). Any of these data points collected could very well be outliers when compared to a city's typical weather. 
