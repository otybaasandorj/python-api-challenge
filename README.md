# python-api-challenge

## WeatherPy

In the python script visualizing the weather of over 500 cities of varying distances from the equator, my script generated 593 results. After converting the cities weather data into a Pandas DataFrame, we ended up with 574 cities. Using Pandas, we are able to showcase the following relationships between latitude vs the max temperature/ humidity/ cloudiness/ and wind speed. 

In the following images, we have created 2 separate DataFrames: one for the northern hemisphere and one for the southern hemisphere. In plotting out the regression line as well as computing the r^2 value, the r^2 value for the Northern Hemisphere (0.687) is higher than for the Southern Hemisphere (0.527), indicating that latitude has a stronger influence on temperature in the Northern Hemisphere. The relationship between increasing latitude and decreasing temperature is clearer in the north. In the Northern Hemisphere, the slope of the line is negative, indicating that as you move further north, temperatures decrease. In the Southern Hemisphere, the slope is positive, meaning temperatures increase as you move from the southern latitudes closer to the equator. In both hemispheres, latitude explains a considerable amount of the variation in temperature, although it’s stronger in the Northern Hemisphere.

![northern_lat_temp](https://github.com/otybaasandorj/python-api-challenge/blob/main/WeatherPy/output_data/images/northern_lat_temp.png)
![southern_lat_temp](https://github.com/otybaasandorj/python-api-challenge/blob/main/WeatherPy/output_data/images/southern_lat_temp.png)

As for the latitude vs humidity, the r^2 values are extremely low in both hemispheres, indicating that latitude does not significantly explain or predict humidity. The near-horizontal regression lines and the low r^2 values suggest that factors other than latitude are likely responsible for the variation in humidity.

![northern_lat_humidity](https://github.com/otybaasandorj/python-api-challenge/blob/main/WeatherPy/output_data/images/northern_lat_humidity.png)
![southern_lat_humidity](https://github.com/otybaasandorj/python-api-challenge/blob/main/WeatherPy/output_data/images/southern_lat_humidity.png)

Moving on to latitude vs cloudiness in the next two images, there is no discernible relationship between latitude and cloudiness in the northern hemisphere, as reflected by the near-zero r^2 value and flat regression line. In the southern hemisphere, there is a slight positive correlation, but it is very weak. Latitude has a minor influence on cloudiness, but other factors likely play a much larger role in determining cloudiness levels.

![northern_lat_cloudiness](https://github.com/otybaasandorj/python-api-challenge/blob/main/WeatherPy/output_data/images/northern_lat_cloudiness.png)
![southern_lat_cloudiness](https://github.com/otybaasandorj/python-api-challenge/blob/main/WeatherPy/output_data/images/southern_lat_cloudiness.png)

Lastly, when looking at latitude vs wind speed, in both the Northern Hemisphere and Southern Hemisphere, the r^2 values are very low, meaning that latitude is not a strong predictor of wind speed. The trends (positive in the Northern Hemisphere, negative in the Southern Hemisphere) are very weak, and the slopes of the lines are small. This indicates that wind speed is likely influenced by other factors rather than latitude alone. 

![northern_lat_windspeed](https://github.com/otybaasandorj/python-api-challenge/blob/main/WeatherPy/output_data/images/northern_lat_windspeed.png)
![southern_lat_windspeed](https://github.com/otybaasandorj/python-api-challenge/blob/main/WeatherPy/output_data/images/southern_lat_windspeed.png)

## VacationPy

Using the data we gathered in the previous notebook, WeatherPy, we are able to plan future vacations. Narrowing down ideal conditiions such as setting our maximum temperature to 90 degrees, cloudiness less than 50%, or less wind speed and humidity, we created another DataFrame to find the closest hotels in our desired cities. What started as a world map of over 500 cities, we were able to narrow down to cities/hotels that match our ideal conditions for a vacation as in the maps. 
