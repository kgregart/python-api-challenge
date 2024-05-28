# python-api-challenge

![sun](https://github.com/kgregart/python-api-challenge/blob/main/Images/sun.jpg)

# Background

Deploying the true power of data use Python requests, APIs, and JSON traversals to answer a fundamental question: "What is the weather like as we approach the equator?" Though it may seem obvious, if pressed for more information, how would you prove that?

# Instructions

This activity is broken down into two deliverables, WeatherPy and VacationPy.

## Part 1: WeatherPy

Using a Python script to visualize the weather of over 500 cities of varying distances from the equator, create a representative model of weather across the cities.

### Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude

Use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Then create a series of scatter plots to showcase the following relationships:

  - Latitude vs. Temperature

  - Latitude vs. Humidity

  - Latitude vs. Cloudiness

  - Latitude vs. Wind Speed

### Requirement 2: Compute Linear Regression for Each Relationship

Compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). Define a function in order to create the linear regression plots.

Create a series of scatter plots and include the linear regression line, the model's formula, and the r values.

_Sample scatter plot with the linear regression line._

Create the following plots:

  - Northern Hemisphere: Temperature vs. Latitude

  - Southern Hemisphere: Temperature vs. Latitude

  - Northern Hemisphere: Humidity vs. Latitude

  - Southern Hemisphere: Humidity vs. Latitude

  - Northern Hemisphere: Cloudiness vs. Latitude

  - Southern Hemisphere: Cloudiness vs. Latitude

  - Northern Hemisphere: Wind Speed vs. Latitude

  - Southern Hemisphere: Wind Speed vs. Latitude

After each pair of plots, explain what the linear regression is modeling. Describe any relationships that you notice and any other findings you may uncover.

## Part 2: VacationPy

Use the Geoapify API and the geoViews Python library to create map visualizations.

__Steps:__

1. Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.

_Humidity map_

2. Narrow down the city_data_df DataFrame to find the ideal weather condition. For example:

    - A max temperature lower than 27 degrees but higher than 21

    - Wind speed less than 4.5 m/s

    - Zero cloudiness

3. Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

4. For each city, use the Geoapify API to find the first hotel located within 10,000 meters of the coordinates.

5. Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image:

_Hotel map_
