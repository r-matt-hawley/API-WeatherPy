# What's the Weather Like?

## Background
This Python project makes calls to the Open Weather Map API to retrieve current weather conditions from about 600 international cities and plots their temperature, cloudiness, wind speed and humidity according to the city's latitude.

## Process
Using Numpy's random number generator and the Citipy module, I created 1500 latitude and longitude locations and found the nearest city.  Then, I queried the Open Weather Map API using this list of cities.  Unfortunately, the API only allows 60 calls per minute (with the free version), so I used the time module to space out the calls.  Finally, I used Matplotlib to plot the results by latitude to visualize weather trends.

## Results
