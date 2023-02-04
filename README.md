# python-api-challenge
## Summary 


The following data was collected to visualize the weather of over 500 cities of varying distances from the equator. 
I used the citypy Python library and the OpenWeatherMap API to help create a representative model of weather across cities. A series of scatter plots were created to showcase the following relationships:
* Latitude vs. Temperature
* Latitude vs. Humidity
* Latitude vs. Cloudiness
* Latitude vs. Wind Speed


The data was split into Northern and Southern Hemisphere and linear regression models were added to the scatter plots to created a visual representation of any possible trends. 
After creating a DataFrame with the information gathered from the various cities (City, Country, Latitude, Longitude, Max Temp, Humidity, Cloudiness, Windspeed and Date collected), this information was used to help plan future vacations. 
Using Jupyter notebook, geoViews Python library and the Geoapify API map visualizations were created to represent all cities from the DataFrame. 
The results were then narrowed down based on temperature and humidity preferences.
Hotels in each city that met the criteria were found and a new map was created that can be used to find this information. 
