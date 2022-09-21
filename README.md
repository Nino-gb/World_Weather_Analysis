# World_Weather_Analysis

## Overview 

Apply analyses, visualizations, statistical skills and API data retrieval from weather data to help customers to filter the data for their weather preferences, which will be used to identify potential travel destinations and nearby hotels. To perform this task we need to collect and present data for customers via the search page which they will then filter base of their preferred travel criteria in order to find the ideal hotel anywhere in the world.

First, we create a Pandas DataFrame with 500 or more of the world's unique cities and their weather data in real time. We will be using Jupyter Notebook and a citypy module to get the cities from latitude and longitude then we perform request on the open weather map API and retrieve the JSON weather data from the cities.

## Analysis Stages:

### 1. Collect the Data
- Use the NumPy module to generate more than 2,000 random latitudes and longitudes.
- Use the citipy module to list the nearest city to the latitudes and longitudes.
- Use the OpenWeatherMap API to request the current weather data from each unique city in your list.
- Parse the JSON data from the API request.
- Collect the following data from the JSON file and add it to a DataFrame:
	-City, country, and date
	-Latitude and longitude
	-Maximum temperature
	-Humidity
	-Cloudiness
	-Wind speed

### 2. Exploratory Analysis with Visualization
- Create scatter plots of the weather data for the following comparisons:
	- Latitude versus temperature
	- Latitude versus humidity
	- Latitude versus cloudiness
	- Latitude versus wind speed
- Determine the correlations for the following weather data:
	- Latitude and temperature
	- Latitude and humidity
	- Latitude and cloudiness
	- Latitude and wind speed
- Create a series of heatmaps using the Google Maps and Places API that showcases the following:
	- Latitude and temperature
	- Latitude and humidity
	- Latitude and cloudiness
	- Latitude and wind speed

### 3. Visualize Travel Data

- Create a heatmap with pop-up markers that can display information on specific cities based on a customer's travel preferences. Complete these steps:
	1. Filter the Pandas DataFrame based on user inputs for a minimum and maximum temperature.
	2. Create a heatmap for the new DataFrame.
	3. Find a hotel from the cities' coordinates using Google's Maps and Places API, and Search Nearby feature.
	4. Store the name of the first hotel in the DataFrame.
	5. Add pop-up markers to the heatmap that display information about the city, current maximum temperature, weather description, and a hotel in the city.
  6. Use loc method to create DataFrames for each city on travel route.
  7. Create a direction layer map for the itinerary route based on customer preferences.
  
> *Marker layer map with a pop-up marker for each city*
![WeatherPy_vacation_map](https://user-images.githubusercontent.com/110786136/191612882-c54d4cda-3037-4399-bd80-acbbe93de818.png)

> *Directions layer map example*
![WeatherPy_travel_map](https://user-images.githubusercontent.com/110786136/191612917-7545a269-be27-4604-a038-ea1bc7453a88.png)
