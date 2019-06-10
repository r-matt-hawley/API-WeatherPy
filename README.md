# What's the Weather Like?

## Background
This Python project makes calls to the Open Weather Map API to retrieve current weather conditions from about 600 international cities and plots their temperature, cloudiness, wind speed and humidity according to the city's latitude.

## Process
Using Numpy's random number generator and the Citipy module, I created 1500 latitude and longitude locations and found the nearest city.  Then, I queried the Open Weather Map API using this list of cities.  Unfortunately, the API only allows 60 calls per minute (with the free version), so I used the time module to space out the calls.  Finally, I used Matplotlib to plot the results by latitude to visualize weather trends.

## Results
* Overall, cities within 20 degrees of the equater appear to have warmer weather than cities further than 20 degrees of the equator.
* At first glance northern cities appear to have significantly lower temperatures than southern cities. However, it appears that there are no cities that are more than 60 degrees south of the equator, whereas the northern limit appears to be 80 degrees. Even excluding the cities that are above 60 degrees latitude, northern cities tend to be colder than southern cities. Collecting data during the spring or fall might correct this bias.
* Latitude appears to have little effect on humidity, cloudiness, and wind speed. However, it is interesting that most cities have more than 60% humidity.
