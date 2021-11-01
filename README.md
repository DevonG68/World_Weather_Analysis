# World_Weather_Analysis
APIs Module 6 Challenge 

Background
Use APIs to visualize weather data over 500 cities by conducting analysis, display visualizations, use of statistical skills, and API Data retrieval with storage of data in a dataframe. 

Project Overview
PlanMyTrip app Is a new product, with company who recommended a few changes to take the app to the next level. Specifically, recommend adding the weather description to the weather data already retrieved in this module. Test input statements to filter the data for their weather preferences (maximum and minimum desired temperature, wind speed, humidity, cloudiness, and current weather descriptions), which will be used to identify potential travel destinations and nearby hotels. From the list of potential travel destinations, the beta tester will choose four cities to create a travel itinerary. Finally, using the Google Maps Directions API, to create a travel route between the four cities as well as a marker layer map.

Resources Used

Python and Pandas Library and modules, Jupyter Notebook, CitiPy, OpenWeatherMap API, GoogleMaps Cloud Platform API, and JSON Traversals

Assignments

Assignment 1: Retrieve Weather Data
Generate a set of 2,000 random latitudes and longitudes, retrieve the nearest city, and perform an API call with the OpenWeatherMap. In addition to the city weather data you gathered in this module, use your API skills to retrieve the current weather description for each city. Then, create a new DataFrame containing the updated weather data.


1.	Create a folder called Weather_Database
 
2.	Create a new Jupyter Notebook file to retrieve the weather data, and name it Weather_Database.ipynb.
 
3.	Create a new set of 2,000 random latitudes and longitudes.
 [image](https://user-images.githubusercontent.com/85171897/139625281-358d1164-2ddc-4a39-8845-a0a15d914006.png)
4.	Get the nearest city using the citipy module.
5.	![image](https://user-images.githubusercontent.com/85171897/139625307-964f0256-49dd-4cf0-839b-6283fa09847b.png)

 
5.	Perform an API call with the OpenWeatherMap.
 ![image](https://user-images.githubusercontent.com/85171897/139625352-adcdf32a-54c9-4ceb-844f-c9e159c7c98b.png)

6.	Retrieve the following information from the API call:
a.	Latitude and longitude
b.	Maximum temperature
c.	Percent humidity
d.	Percent cloudiness
e.	Wind speed
f.	Weather description (for example, clouds, fog, light rain, clear sky)
![image](https://user-images.githubusercontent.com/85171897/139625375-5d8a8a8a-aac9-478d-8317-76270fa71a86.png)




Assignment 2: Create a Customer Travel Destinations Map
1.	Create a folder called Vacation_Search.
 
2.	Download the Vacation_Search_starter_code.ipynb file into your Vacation_Search folder, and rename it Vacation_Search.ipynb.
3.	In the Vacation_Search.ipynb file, make sure the dependencies and API keys are imported correctly.
 
4.	Use the instructions below to add code where indicated by the numbered-step comments in the starter code file.
5.	In Step 1, import the WeatherPy_Database.csv file from your Weather_Database folder from Deliverable 1 as a DataFrame.

![image](https://user-images.githubusercontent.com/85171897/139625407-e9e06442-c036-44a4-ba15-49919bb90157.png)

 
6.	In Step 2, write two input statements that prompt the user to enter their minimum and maximum temperature criteria for their vacation.
7.![image](https://user-images.githubusercontent.com/85171897/139625428-ee7ab91d-52ef-429b-ac0c-0c02f3bdf84f.png)

 
7.	In Step 3, use the loc method to filter the city_data_df DataFrame for temperature criteria collected in Step 2, then create a new DataFrame.
 ![image](https://user-images.githubusercontent.com/85171897/139625448-86f64bd0-dd0b-4635-93ea-b9165b80bd94.png)

8.	In Steps 4a-b, determine if there are any empty rows, then drop them if necessary and create a new DataFrame.
 ![image](https://user-images.githubusercontent.com/85171897/139625460-df49eaa6-2fcc-40ed-b349-3c7a68dc0f3e.png)

9.	In Steps 5a-b, use the provided code to create a new DataFrame, hotel_df, that will hold the hotel names from the hotel search in Steps 6a-6f.

![image](https://user-images.githubusercontent.com/85171897/139625475-f11f6963-bf13-4ff6-852c-438427d722fb.png)

 
10.	In Step 6a, we have supplied the search parameters, which are the same as in this module, that you’ll need to use to search for a hotel for each city in Steps 6b-f.

12.	In Steps 6b-f, iterate through the hotel_df DataFrame, retrieve the latitude and longitude of each city to find the nearest hotel based on the search parameters from Step 6a, then add the hotel name to the hotel_df DataFrame. If a hotel isn't found, skip to the next city.
 ![image](https://user-images.githubusercontent.com/85171897/139625496-4caa4eec-4d83-4384-8530-59a02999f24d.png)


12.	In Step 7, drop any rows in the hotel_df DataFrame where a hotel name is not found.
1.	Before exporting your DataFrame as a CSV, take a moment to confirm that your hotel_df DataFrame looks similar to the image below.
 ![image](https://user-images.githubusercontent.com/85171897/139625518-5c4ccfbc-bb1f-4db8-94bc-4c1571dd9a92.png)


1.	Create a Travel Itinerary Map

![image](https://user-images.githubusercontent.com/85171897/139625204-0fab335a-cec2-417b-b3d7-65b6c2a79636.png)
