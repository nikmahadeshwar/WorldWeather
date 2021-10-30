# World_Weather_Analysis

## Project Overview
This project illustrates analysis, visualization, and statistical skills by retrieving and analyzing weather data for a hypothetical travel company, PlanMyTrip. We are using Python, decision and repetition statements, data structures, Pandas, Matplotlib, and SciPy statistics.

## Resources
Data Source: https://openweathermap.org/api

## Software:
Jupyter Notebook, Pandas Library, CityPy, Python Request, APIs, JSON Traversals

## Summary
Summary is as follows:

* Performing tasks using Python libraries and modules.
* Retrieving data from an API “get” request to a server.
* Retrieving and store values from a JSON array.
* Using try and except blocks to resolve errors.
* Writing Python functions.
* Creating scatter plots using the Matplotlib library, and apply styles and features to a plot.
* Performing linear regression, and add regression lines to scatter plots.
* Creating heatmaps, and add markers using the Google Maps API.


## Objectives:
* Use nested try-except blocks
* Use Pandas methods and attributes on a DataFrame or Series.
* Create a new DataFrame from a new API search with new weather parameters.
* Filter DataFrames based on input and nested decision statements, and logical expressions.
* Create pop-up markers on a Google map from a filtered DataFrame.
* Add a directions layer on a Google map between cities in the filtered DataFrame.

## Challenge Summary

## Weather Description and Amount of Precipitation for Each City
We used a set of 1,500 random latitudes and longitudes.
Got the nearest city using the citipy module.
Performed an API call with the OpenWeatherMap.
Retrieved the following information from the API call:

* Latitude and longitude
* Maximum temperature
* Percent humidity
* Percent cloudiness
* Wind speed
* Weather description (e.g. clouds, fog)
* Using a try-except block, if it is raining, get the amount of rainfall in inches for the last three hours. If it is not raining, add 0 inches for the city
* Using a try-except block, if it is snowing, get the amount of snow in inches for the last three hours. If it is not snowing, add 0 inches for the city. Added the data to a   
  new DataFrame.

Our new DataFrame looks similar to the following image:

WeatherPy_challenge DataFrame



From the filtered DataFrame we added the cities to a marker layer map with a pop-up marker for each city that includes:
* Hotel name
* City
* Country
* Current weather description with the maximum temperature
![alt text](https://github.com/nikmahadeshwar/WorldWeather/blob/main/WeatherPy_vacation.png)

## Travel Itinerary with a Corresponding Map
We created a map (travel itinerary) that shows the route between four cities from the customer’s possible travel destinations, and then created a map with pop-up markers for the four cities, by:

Importing the WeatherPy_vacation.csv file as a new DataFrame. From the vacation search map, we chose four cities in close proximity on our map that are on the same continent that a customer might travel to, and then created a directions layer map.

* We Filtered the DataFrame for each city we wanted to go to and created separate DataFrames for each city.
* Used the directions Layer instructions from the gmaps documentation
* Use the list indexing and Pandas methods to get the latitude-longitude pairs for each city DataFrame as tuples.

![alt text](https://github.com/nikmahadeshwar/WorldWeather/blob/main/WeatherPy_travel_map_markers.png)

For the travel_mode, we used either DRIVING, BICYCLING, or WALKING.
![alt text](https://github.com/nikmahadeshwar/WorldWeather/blob/main/WeatherPy_travel_map.png)
