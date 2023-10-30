# python-api-challenge
Using Python requests, APIs, and JSON traversals to answer a fundamental question:  What is the weather like as we approach the equator

## Add a .gitignore File
For this assignment, you will need to add a .gitignore file to your repo.
Before adding your files to GitHub, add api_keys.py to the .gitignore file by following these steps:
   1. Open your python-api-challenge GitHub folder in VS Code.
   2. Open the .gitignore file and type the following code on the first line:
      ![Screen Shot 2023-10-22 at 9 48 23 PM](https://github.com/dilqvl62/python-api-challenge/assets/107519883/74928780-49b6-481c-8e1d-0c090d059013)

# Objectives 
This activity is broken down into two deliverables, WeatherPy and VacationPy.
## Part 1: WeatherPy
In this deliverable, you'll create a Python script to visualize the weather of over 500 cities of varying distances from the equator. You'll use the [citipy Python library](https://pypi.org/project/citipy/), [the OpenWeatherMap API](https://openweathermap.org/api),  to create a representative model of weather across cities.

* Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
   To fulfill the first requirement, you'll use the OpenWeatherMap API to retrieve weather data from the cities list generated using the following code .
   ![Screen Shot 2023-10-22 at 10 20 38 PM](https://github.com/dilqvl62/python-api-challenge/assets/107519883/bd5a514a-fc0b-44eb-8407-99d27e7fef46)

  Next, I'll create a series of scatter plots to showcase the following relationships:

   * [Latitude vs. Temperature](https://github.com/dilqvl62/python-api-challenge/blob/main/output_data/Fig1.png) 
   * [Latitude vs. Humidity](https://github.com/dilqvl62/python-api-challenge/blob/main/output_data/Fig2.png)
   * [Latitude vs. Cloudiness](https://github.com/dilqvl62/python-api-challenge/blob/main/output_data/Fig3.png)
   * [Latitude vs. Wind Speed](https://github.com/dilqvl62/python-api-challenge/blob/main/output_data/Fig4.png)
 
* Requirement 2: Compute Linear Regression for Each Relationship

  Define a function in order to create the linear regression plots.
![Screen Shot 2023-10-22 at 10 41 47 PM](https://github.com/dilqvl62/python-api-challenge/assets/107519883/198dc69b-541e-4a7d-b309-6046b3f76487)

Next, create a series of scatter plots. The linear regression line, the model's formula, and the r values as you can see in the following images:
 * Northern Hemisphere: [Temperature vs. Latitude](https://github.com/dilqvl62/python-api-challenge/blob/main/output_data/Temperature%20vs.%20Latitude.png)
   
 * Southern Hemisphere: [Temperature vs. Latitude](https://github.com/dilqvl62/python-api-challenge/blob/main/output_data/Temp%20vs.%20Lat.png)
   
 * Northern Hemisphere: [Humidity vs. Latitude](https://github.com/dilqvl62/python-api-challenge/blob/main/output_data/Latitude%20vs%20Humidity%20(NH).png)
   
 * Southern Hemisphere: [Humidity vs. Latitude](https://github.com/dilqvl62/python-api-challenge/blob/main/output_data/Lat%20vs%20Humidity%20(SH).png)
   
 * Northern Hemisphere: [Cloudiness vs. Latitude](https://github.com/dilqvl62/python-api-challenge/blob/main/output_data/Cloudiness%20vs%20latitude%20(NH).png)
   
 * Southern Hemisphere: [Cloudiness vs. Latitude](https://github.com/dilqvl62/python-api-challenge/blob/main/output_data/Cloudiness%20vs%20latitude%20(SH).png)
   
 * Northern Hemisphere: [Wind Speed vs. Latitude](https://github.com/dilqvl62/python-api-challenge/blob/main/output_data/Latitude%20vs%20windSpeed%20(NH).png)
   
 * Southern Hemisphere: [Wind Speed vs. Latitude](https://github.com/dilqvl62/python-api-challenge/blob/main/output_data/Latitude%20vs%20windSpeed%20(SH).png)

## Part 2: VacationPy
use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualizations.

1. Create a map that displays a point for every city in the city_data_df DataFrame. The size of the point should be the humidity in each city.
   
  ![Screen Shot 2023-10-22 at 11 32 06 PM](https://github.com/dilqvl62/python-api-challenge/assets/107519883/14c1204c-13e5-4605-9205-d40eefeb4bdf)

2. Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

3. For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.

4. Add the hotel name and the country as additional information in the hover message for each city on the map:

![Screen Shot 2023-10-22 at 11 34 21 PM](https://github.com/dilqvl62/python-api-challenge/assets/107519883/70529d07-7f4f-445c-b39d-f3752c22ab92)



      


