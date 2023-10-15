# Python API Challenge

This project aims to analyze weather data of various cities to understand the relationship between weather variables and the latitude of the cities. We also utilize the analyzed data to plan future vacations by selecting ideal weather conditions for our trip and finding hotels in the cities that meet our criteria.

# Part 1: WeatherPy

In this part, we create a Python script to visualize the weather of over 500 cities of varying distances from the equator using the `citipy` Python library, the OpenWeatherMap API, and our problem-solving skills.

To fulfill the first requirement, we'll use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, we'll create a series of scatter plots to showcase the following relationships:

- Latitude vs. Temperature
- Latitude vs. Humidity
- Latitude vs. Cloudiness
- Latitude vs. Wind Speed


![image 1](https://github.com/isekmen/python-api-challenge/assets/101214487/e749b035-cf87-463d-b107-eb7db337b024)





We also compute linear regression for each relationship, separating the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude).

We should create the following plots:

Northern Hemisphere: Temperature vs. Latitude
Southern Hemisphere: Temperature vs. Latitude
Northern Hemisphere: Humidity vs. Latitude
Southern Hemisphere: Humidity vs. Latitude
Northern Hemisphere: Cloudiness vs. Latitude
Southern Hemisphere: Cloudiness vs. Latitude
Northern Hemisphere: Wind Speed vs. Latitude
Southern Hemisphere: Wind Speed vs. Latitude

### Part 2: VacationPy

In this part, we use our weather data to plan future vacations. We use Jupyter notebooks, the `geopandas` Python library, and the Geoapify API to create map visualizations of our ideal vacation spots.

The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 is provided to help us get started.
Our main tasks will be to use the Geoapify API and the geoViews Python library and employ our Python skills to create map visualizations.
To succeed on this deliverable of the assignment, open the `VacationPy.ipynb` starter code and complete the following steps:


Create a map that displays a point for every city in the `city_data_df` DataFrame as shown in the following image. The size of the point should be the humidity in each city.

![image 2](https://github.com/isekmen/python-api-challenge/assets/101214487/36e5ee2b-ebfd-4bf1-9d47-246df461cfb1)





Narrow down the city_data_df DataFrame to find your ideal weather condition. For example:
A max temperature lower than 27 degrees but higher than 21
Wind speed less than 4.5 m/s
Zero cloudiness

Create a new DataFrame called `hotel_df` to store the city, country, coordinates, and humidity.

For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.

Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image:

![image 3](https://github.com/isekmen/python-api-challenge/assets/101214487/d232bda8-e4ea-4686-a6e0-6bee87aa4dc6)




