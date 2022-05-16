# World_Weather_Analysis
Resources

    - Python 3.9.7
    - Jupyter Notebook
    - Google Maps Platform:
        - Places API
        - Directions API
    - OpenWeatherMap API:
        - Current weather data
    - Jupyter-gmaps
        - Weighted Heatmaps
        - Markers and symbols
        - Directions layer
    - Citipy module
    - Pandas
    - NumPy
    - Matplotlib

## Overview

PlanMyTrip is a project that employs API interactions to provide real-time suggestions to users for destinations based on ideal weather preferences.   By collecting and analyzing global data and monitoring weather parameters, this project offers visualizations with which the user can discover and make travel decisions such as destination, lodging, current weather, and trip itinerary.  

## Process

- From over 1500 random generated NumPy arrays and zipped latitude and longitude coordinates, more than 500 cities were identified and named.  
- Weather data was gathered from the above APIs list in the form of JSON files, further parsed and repackaged into a pandas dataframe and csv file.  
- The implementation of linear regression models using matplotlib helped to identify a correlation between Latitude coordinates and maximum temperature.  No other parameters showed similar results. 
- Heatmaps were generated reflecting the weather parameters using gmaps.
- Google's Maps and Places API, Nearby Search, provided Hotel names for city coordinates.
- Pop-up markers display hotel name, city name, current weather description and maximum temperature.

**Heatmap for Maximum Temperature**

![Screen Shot 2022-05-16 at 10 30 02 AM](https://user-images.githubusercontent.com/100544761/168629735-d90c3b16-1d9b-4ed9-ab45-db2cbcec41e0.png)

**API get request code snippet**

![Screen Shot 2022-05-16 at 10 31 07 AM](https://user-images.githubusercontent.com/100544761/168629875-99e0e229-e953-4042-a56c-3938d56257b7.png)

**Markers and Content Box**

![Screen Shot 2022-05-16 at 10 34 55 AM](https://user-images.githubusercontent.com/100544761/168630600-66339c8b-3162-4c47-9d14-fc7a709f0816.png)

**Linear Regression models**

![Fig5](https://user-images.githubusercontent.com/100544761/165880471-20f7cd3a-d5f9-4e64-9e18-5167a35a75ce.png)

![Fig6](https://user-images.githubusercontent.com/100544761/165880479-a9f96953-6df9-4b5c-b62a-d33715c233d5.png)

 **Finally, a small list of destinations were chosen to create a travel itinerary using Google's Direction API in the form of a map with markers and info boxes**

![WeatherPy_travel_map_markers](https://user-images.githubusercontent.com/100544761/165880391-826d0726-520a-4246-b46a-e7223ca3566f.png)

![Screen Shot 2022-05-16 at 10 44 35 AM](https://user-images.githubusercontent.com/100544761/168632104-12267b65-5597-498d-9ea6-3a921d0e7184.png)
