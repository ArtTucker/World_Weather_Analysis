# World Weather Analysis
Gathering weather and travel information with with OpenWeatherMap and Google Maps APIs

This project was built around providing functionality to an app called **PlanMyTrip**. The key deliverables were:
- retrieve weather data from the OpenWeatherMap.org API;
- create a map of potential travel destinations using the Google Map API, based on customer's temperature preference input;
- create a travel itinerary map, using Google Maps Directions API and a selection of four destinations.

### The first deliverable
... is contained within the [Weather_Database](https://github.com/ArtTucker/World_Weather_Analysis/tree/main/Weather_Database) subfolder. The primary purpose of this code is to:
- create a random list of 2000 latitude/longitude pairs;
- from those coordinate, create a list of cities which are 'nearby' and are not duplicated;
- pull current weather data for all the cities on the list (temp, humidity, cloudiness, wind speed, and weather description);
- export this data to a csv file to be used later.

### The second deliverable
... is contained within the [Vacation_Search](https://github.com/ArtTucker/World_Weather_Analysis/tree/main/Vacation_Search) subfolder. This code uses the city and weather data contained in the previously created csv file. It preforms the following actions:
- takes weather range inputs from the user on minimum and maximum temperatures, and uses those figures to refine the list of cities;
- uses the Google Maps Nearby search API to find hotels in the refined list of cities;
- uses the Google Maps API to create a map and marker layer showing all potential travel destinations.
![WeatherPy Travel Destinations](Vacation_Search/WeatherPy_vacation_map.png)

### The third and final deliverable
... is contained within the [Vacation_Itinerary](Vacation_Itinerary) subfolder. 