## Planning a vacation with data
* Which locations have the best weather in mid-October? 
* Where can I stay? 

Let's start at the top ... or the bottom ...

Northern Hemisphere or Southern Hemisphere? 

How does latitude affect weather parameters such as temperature, humidity, cloudiness, and wind speed? We took a random sampling of 605 cities across the globe, and compared them in terms of latitude versus current weather data. Weather data was collected on 10/27/2020 from the Open Weather API by an analyst based in the eastern United States.  

![City Latitude vs. Max Temperature (F) Scatter Plot](/WeatherPy/Images/latitudeVStemp.png)

### 1. Scatter plot observation: City Latitude vs. Max Temperature (F)

The scatter plot above shows the relationship between latitude and the maximum temperature (F) of a city. Cities closer to the equator and in the southern hemisphere have a higher maximum temperature than those further north.

---

![City Latitude vs. Humidity (%) Scatter Plot](/WeatherPy/Images/latitudeVShumidity.png)

### 2. Scatter plot observation: City Latitude vs. Humidity

The scatter plot above shows that there's a weak relationship between a city's latitude and humidity. 

---

![City Latitude vs. Cloudiness (%) Scatter Plot](/WeatherPy/Images/latitudeVScloudiness.png)

### 3. Scatter plot observation: City Latitude vs. Cloudiness

The scatter plot above shows that there is no relationship between a city's latitude and cloudiness. 

---

![City Latitude vs. Wind Speed (mph) Scatter Plot](/WeatherPy/Images/latitudeVSwindspeed.png)

### 4. Scatter plot observation: City Latitude vs. Wind Speed
The scatter plot above shows there is no relationship between wind speed and a city's latitude. A few outliers can be seen with high wind speeds, but as this data is a snapshot of weather events on a single date, this is not a reliable indication of a strong relationship between these variables. 

---
### Comparing the Northern and Southern Hemispheres

**Northern Hemisphere** | **Southern Hemisphere**
--------------------- | ---------------------
![Northern Hemisphere City Latitude vs. Max Temperature](/WeatherPy/Images/n_hemi_latitudeVStemp.png) | ![Southern Hemisphere City Latitude vs. Max Temperature](/WeatherPy/Images/s_hemi_latitudeVStemp.png)
![Northern Hemisphere City Latitude vs. Humidity (%)](/WeatherPy/Images/n_hemi_latitudeVShumidity.png) | ![Southern Hemisphere City Latitude vs. Humidity (%)](/WeatherPy/Images/s_hemi_latitudeVShumidity.png)
![Northern Hemisphere City Latitude vs. Cloudiness (%)](/WeatherPy/Images/n_hemi_latitudeVScloudiness.png) | ![Southern Hemisphere City Latitude vs. Cloudiness (%)](/WeatherPy/Images/s_hemi_latitudeVScloudiness.png) 
![Northern Hemisphere City Latitude vs. Wind Speed (mph)](/WeatherPy/Images/n_hemi_latitudeVSwindspeed.png) | ![Southern Hemisphere City Latitude vs. Wind Speed (mph)](/WeatherPy/Images/s_hemi_latitudeVSwindspeed.png)

---
### Defining parameters to find locations with ideal weather conditions: 
1. Temperatures between 72-78 degrees Fahrenheit
2. Humidity below 80%
3. Cloudiness less than 25%
4. Wind Speed below 5 mph

Let's visualize locations that meet our criteria on a humidity heatmap: 

![Humidity Heatmap with ideal locations pinpointed](/VacationPy/Images/humidity_heatmap_with_hotel_markers.png)

Finding a place to stay in ideal locations: 

![Hotel Locations pinpointed with marker info revealed](/VacationPy/Images/hotel_locations_with_marker_info.png)

### Google heatmap with hotel markers observation: 
As shown in the map above, after narrowing down possible vacation locales, most are in areas with moderate humidity. On a personal note, I was pleased to see the city of Wilmington, NC included. It's a place I know well from my four years attending UNC-Wilmington. I can personally recommend Wilmington as a pleasant place to visit, which boosts my confidence that the other locations would have great weather for traveling as well. 