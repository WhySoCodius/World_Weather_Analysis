# World_Weather_Analysis
Assist PlanMyTrip, a travel technology business, in analysing customer data via a search page so that clients can locate their preferred hotel around the world.

## Overview of the Analysis
Analyzed 675 cities throughout the world and filtered out a favourite vacation place for customers based on their chosen city's temperature and developed an itinerary.

## Resources
### Data Sources: 
[Cities](/weather_data/cities.csv) and [Weather Data](/Vacation_Search/WeatherPy_vacation.csv) are used for analysis to help customer plan Vacation spot and Itinerary.

### Software:
[![Anaconda-Server Badge](https://anaconda.org/conda-forge/terraform-provider-github/badges/version.svg)](https://anaconda.org/conda-forge/terraform-provider-github)
[![PyPI - Python](https://img.shields.io/pypi/pyversions/iconsdk?logo=pypi)](https://pypi.org/project/iconsdk)
[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)


## Results

### Weather Database

Using a Jupyter notebook, created a [Database](/Weather_Database/WeatherPy_Database.csv) of random Latitude and Longitude coordinates representing various cities around the world, and then used the [OpenWeather API](https://openweathermap.org/api) to create data such as maximum temperature, Humidity, Cloudiness, Wind speed, and current weather description for those cities.

![Max Temperature](/weather_data/Fig1.png) ![Humidity](/weather_data/Fig2.png)
![Cloudiness](/weather_data/Fig3.png) ![Wind Speed](/weather_data/Fig4.png)


### Vacation Search

The next step was to generate a [New Database](/weather_data/cities.csv) by filtering out the Vacation Spots using the above database and the customers' preferred maximum and minimum temperatures.
Also, using the Google Maps Platform APIs, created a [marker layer](https://developers.google.com/maps/documentation/javascript/markers) to plot the desired vacation sites around the world as well as the hotels in those locations.

![WeatherPy_vacation_map](/Vacation_Search/WeatherPy_vacation_map.png)


### Vacation Itinerary

Finally, from the new Database we chose 4 cities and create an Itinerary to travel keeping the desirable weather conditions.

![WeatherPy_travel_map](/Vacation_Itinerary/WeatherPy_travel_map.png?raw=true)

Chose "Driving" as the mode of travel and added marker layer and description of Hotel and weather condition for easy giude during the Vacation.

![WeatherPy_travel_map_markers](/Vacation_Itinerary/WeatherPy_travel_map_markers.png)
