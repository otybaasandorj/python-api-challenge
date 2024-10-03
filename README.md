# python-api-challenge

## WeatherPy

In the python script visualizing the weather of over 500 cities of varying distances from the equator, my script generated 593 results. After converting the cities weather data into a Pandas DataFrame, we ended up with 574 cities. Using Pandas, we are able to showcase the following relationships between latitude vs the max temperature/ humidity/ cloudiness/ and wind speed. 

In the following images, we have created 2 separate DataFrames: one for the northern hemisphere and one for the southern hemisphere. In plotting out the regression line as well as computing the r^2 value, the r^2 value for the Northern Hemisphere (0.687) is higher than for the Southern Hemisphere (0.527), indicating that latitude has a stronger influence on temperature in the Northern Hemisphere. The relationship between increasing latitude and decreasing temperature is clearer in the north. In the Northern Hemisphere, the slope of the line is negative, indicating that as you move further north, temperatures decrease. In the Southern Hemisphere, the slope is positive, meaning temperatures increase as you move from the southern latitudes closer to the equator. In both hemispheres, latitude explains a considerable amount of the variation in temperature, although it’s stronger in the Northern Hemisphere.

![northern lat temp](https://github.com/otybaasondorj/python-api-challenge/blob/main/WeatherPy/output_data/images/northern_lat_temp.png) 
![southern lat temp](https://github.com/otybaasondorj/python-api-challenge/blob/main/WeatherPy/output_data/images/southern_lat_temp.png)
