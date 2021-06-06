# world-weather-analysis

This project gathers and maps data about the weather conditions from a set of a few hundred randomized cities around the world using the python citipy module and OpenWeatherMap's API. This information was then used with the Google Maps API to find hotels in each city and plot a hypothetical travel route between four of those cities.

The project was broken into three parts.

## Part 1: Weather Database
Part 1 of the project collected the June 4, 2021 weather conditions of a randomized group of a few hundred cities around the world. This was done by generating a random set of 2000 latitude and longitude coordinates, and finding the nearest cities to each coordinate. The result was a list of 752 cities. Using OpenWeatherMap's API, the weather conditions for each of those cities was gathered, if available. Any cities without weather data were dropped. The end result was compiled into a table of 691 cities and their weather intormation,

[[Link to table]](Weather_Database/WeatherPy_Database.csv)

## Part 2: Vacation Search
Part 2 simply used the Google Maps API to find a hotel in each of the 691 cities, and generated a map with location markers that would pop up an info box about each city when clicked on.

[[Link to map sample image]](Vacation_Search/WeatherPy_vacation_map.png)

## Part 3: Vacation Itinerary
Part 3 of the project selected four random cities and created a round trip travel route between them using gmaps. A map of the travel route was generated, as well as a map with markers that popped up info boxes with information on each of the 4 cities.

[[Link to travel route map]](Vacation_Itinerary/WeatherPy_travel_map.png)

[[Link to marker map]](Vacation_Itinerary/WeatherPy_travel_map_markers.png)

