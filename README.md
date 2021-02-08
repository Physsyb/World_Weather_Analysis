# World_Weather_Analysis
# Basic Project Plan
Here's an outline of your project plan:

* Task: Collect and analyze weather data across cities worldwide.
* Purpose: PlanMyTrip will use the data to recommend ideal hotels based on clients' weather preferences.
* Method: Create a Pandas DataFrame with 500 or more of the world's unique cities and their weather data in real time. This process will entail collecting, analyzing, and visualizing the data. Your analysis of the data will be split into three main parts, or stages.

1. Collect the Data
* Use the NumPy module to generate more than 1,500 random latitudes and longitudes.
* Use the citipy module to list the nearest city to the latitudes and longitudes.
* Use the OpenWeatherMap API to request the current weather data from each unique city in your list.
* Parse the JSON data from the API request.
* Collect the following data from the JSON file and add it to a DataFrame:
  * City, country, and date
  * Latitude and longitude
  *  Maximum temperature
  * Humidity
  * Cloudiness
  * Wind speed
2. Exploratory Analysis with Visualization
* Create scatter plots of the weather data for the following comparisons:
  * Latitude versus temperature
  * Latitude versus humidity
  * Latitude versus cloudiness
  * Latitude versus wind speed
* Determine the correlations for the following weather data:
  * Latitude and temperature
  * Latitude and humidity
  * Latitude and cloudiness
  * Latitude and wind speed
* Create a series of heatmaps using the Google Maps and Places API that showcases the following:
  * Latitude and temperature
  * Latitude and humidity
  * Latitude and cloudiness
  * Latitude and wind speed
3. Visualize Travel Data

Create a heatmap with pop-up markers that can display information on specific cities based on a customer's travel preferences. Complete these steps:
* Filter the Pandas DataFrame based on user inputs for a minimum and maximum temperature.
* Create a heatmap for the new DataFrame.
* Find a hotel from the cities' coordinates using Google's Maps and Places API, and Search Nearby feature.
* Store the name of the first hotel in the DataFrame.
* Add pop-up markers to the heatmap that display information about the city, current maximum temperature, and a hotel in the city.

##  Challenge Question
Jack loves the PlanMyTrip app. Beta testers love it too. And, as with any new product, they’ve recommended a few changes to take the app to the next level. Specifically, they recommend adding the weather description to the weather data you’ve already retrieved in this module. Then, you'll have the beta testers use input statements to filter the data for their weather preferences, which will be used to identify potential travel destinations and nearby hotels. From the list of potential travel destinations, the beta tester will choose four cities to create a travel itinerary. Finally, using the Google Maps Directions API, you will create a travel route between the four cities as well as a marker layer map.
This new assignment consists of three technical analyses. You will submit the following deliverables:
* Deliverable 1: Retrieve Weather Data
* Deliverable 2: Create a Customer Travel Destinations Map
* Deliverable 3: Create a Travel Itinerary Map

##  Resources
* Data File: `WeatherPy_vacation.csv`
* Software: Matplotlib 3.3.2, Python 3.7.9, Jupyter Notebook 6.1.4, Pandas

## Deliverable 1 : Retrieve Weather Data
> Retrieve Weather Data

1. #### Retrieve all of the following information from the API call.
* Latitude and longitude.
* Maximum temperature.
* Percent humidity.
* Percent cloudiness.
* Wind speed.
Weather description (for example, clouds, fog, light rain, clear sky).
![1](https://user-images.githubusercontent.com/76136277/107172740-1e569880-6994-11eb-91b9-0bf0033bfcb7.PNG)

2. #### Add the weather data to a new DataFrame.

![2](https://user-images.githubusercontent.com/76136277/107174855-4b597a00-6999-11eb-8a98-2f0747e4b656.PNG)

3. #### Export the DataFrame as WeatherPy_Database.csv into the Weather_Database folder
![3](https://user-images.githubusercontent.com/76136277/107174892-688e4880-6999-11eb-8ef0-d97220815619.PNG)

## Deliverable 2 : Create a Customer Travel Destinations Map.
1. #### Input statements are written to prompt the customer for their minimum and maximum temperature preferences. (5 pt)
![4](https://user-images.githubusercontent.com/76136277/107175134-0eda4e00-699a-11eb-9914-2f8b590adab1.PNG)

2. #### A new DataFrame is created based on the minimum and maximum temperature, and empty rows are dropped
![5](https://user-images.githubusercontent.com/76136277/107175237-4e089f00-699a-11eb-8c25-4d44a68ea751.PNG)

3.  #### The hotel name is retrieved and added to the DataFrame, and the rows that don’t have a hotel name are dropped.
![7](https://user-images.githubusercontent.com/76136277/107175313-83ad8800-699a-11eb-9d47-94ea931a0bef.PNG)

4. #### The DataFrame is exported as a CSV file into the Vacation_Search folder and is saved as `WeatherPy_vacation.csv`
![8](https://user-images.githubusercontent.com/76136277/107175413-c4a59c80-699a-11eb-8869-4845acb819d3.PNG)

5. #### A marker layer map with pop-up markers for the cities in the vacation DataFrame is created, and it is uploaded as a PNG. Each marker has the following information: 
* Hotel name
* City
* Country
* Current weather description with the maximum temperature
![WeatherPy_vacation_map](https://user-images.githubusercontent.com/76136277/107175506-02a2c080-699b-11eb-91a7-402ef97fc7f9.PNG)

## Deliverable 3 : Create a Travel Itinerary Map
1. #### Four DataFrames are created, one for each city on the itinerary. 
![9](https://user-images.githubusercontent.com/76136277/107175773-adb37a00-699b-11eb-9d12-e837ce37f0ee.PNG)

2. #### The latitude and longitude pairs for each of the four cities are retrieved.
![19](https://user-images.githubusercontent.com/76136277/107176490-89589d00-699d-11eb-9568-49fb1e508767.PNG)


3. #### A directions layer map between the cities and the travel map is created and uploaded as WeatherPy_travel_map.png
![WeatherPy_travel_map](https://user-images.githubusercontent.com/76136277/107176513-9aa1a980-699d-11eb-99b6-77c874d2d80b.png)

4. #### A DataFrame that contains the four cities on the itinerary is created.
![20](https://user-images.githubusercontent.com/76136277/107176625-e5bbbc80-699d-11eb-8634-fb105ac3003c.PNG)

5. #### A marker layer map with a pop-up marker for the cities on the itinerary is created, and it is uploaded as WeatherPy_travel_map_markers.png. Each marker has the following information: 
* Hotel name
* City
* Country
* Current weather description with the maximum temperature
![21](https://user-images.githubusercontent.com/76136277/107176987-bc4f6080-699e-11eb-9f01-5a2bd67fd37d.PNG)
