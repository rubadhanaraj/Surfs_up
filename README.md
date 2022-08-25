# Surfs_up
## Overview of the project
The purpose of this project to do a weather analysis to convince an investor for opening a surf shop which sells surf boards and serves icecreams,in oahu, Hawaii. In order to get the investor for this venture, we need to provide statistical weather analysis  on weather condition in Oahu. For this analysis, we used SQLAlchemy to perform queries from SQLite database to get the information we need for this analysis. In this project, jupyter notebook was used to load and read the data from SQLite database by importing dependencies. Visual Studiop Code was used to write codes in python and create Flask routes for sharing the results in webpage with the investors,by running the Flask app in VS code terminal.

## Results 
For the analysis all the dependencies have been imported and code is appropriately documented. 
* The analysis started with querying the precipitaion data for 12 months from August 23, 2016 - August 23, 2017. The results were,

![image](https://user-images.githubusercontent.com/108298416/186755807-674f4b02-9743-4730-8ecc-cd5a85535aec.png) ![image](https://user-images.githubusercontent.com/108298416/186756739-32f769b9-ad2d-4439-9bb4-c3c5eedf2a78.png)

* Next, the most active stations which were collecting weather data has been listed using groupby function. There were 9 stations in the dataset and USC00519281 station has the most number of entries. The average temperature, the lowest temperature recorded and the highest temperature recorded for this staion id have been calculated. 
The results showed that the highest temperature recorded in the year was 85°F with a low of 54°F and the average temperature throughout the year was 71.6°F

![image](https://user-images.githubusercontent.com/108298416/186759711-ca1d19c1-d245-4a10-ab34-9cbb22c64b14.png)

* The analysis was done further to find the temperature data for the months of June and December in Oahu, in order to determine if the surf and ice cream shop business is sustainable year-round. For this challenge, a query was performed that filters the date column from the Measurement table to retrieve all the temperatures for the month of June and December. Then the temperatures were converted into dataframe for the months of June and December respectively followed by calculating the summary statistics for the respective dataframes.

![image](https://user-images.githubusercontent.com/108298416/186760766-fbddf023-2632-4604-ae33-d3cc43288961.png)  ![image](https://user-images.githubusercontent.com/108298416/186760664-2a96dcfc-75bc-45bf-a376-7815039c5279.png)

The maximum temperatures for the months of June and December were 85°F and 83°F whereas, the mean temperatures for the months of June and December were 75°F and 71°F respectively.

![image](https://user-images.githubusercontent.com/108298416/186771159-539dd120-a701-4e63-845e-94543e055bd5.png)

![image](https://user-images.githubusercontent.com/108298416/186771228-2ae61457-6325-4b97-9db7-190701397d9e.png)



## Summary
1. Along with the temperature statistics for the months of June and December, the precipitation statistics were also calculated by writing additional queries.

![image](https://user-images.githubusercontent.com/108298416/186766014-bea1ba2f-52e3-4c73-9c9a-275a486ade8a.png)

![image](https://user-images.githubusercontent.com/108298416/186766089-04df1457-2ea4-4260-9340-63889825920c.png)

The results shows that the maximum precipitation for the month of June is 4.43 inches and for the month of December is 6.42 inches.

2. Scatter plots were created for the months of June and December for temperatures by precipitations to analyse the weather conditions for opening a surf shop.

![image](https://user-images.githubusercontent.com/108298416/186773662-2a77687a-2e25-4304-8681-5f0755bde009.png)

![image](https://user-images.githubusercontent.com/108298416/186773712-c6895342-939b-4e17-9332-3eaffeb97b67.png)

The results of these analyses show that the weather patterns for the months of June and December were mostly similar. The temperatures and precipitation values for both the months were mostly similar with the differnce of few degrres farenheit. The average temperature for June is  75°F, a little higher than the mean temperature of 71°F for December. However, the average precipitation in December was 0.22 inches whereas June had 0.14 inches. The analysis with the provided data tells that opening a Surf and Ice Cream shop year-round could be a possibility. But there are other variables which needs to be considered, like wind condition and humidity also plays an important role in finding an optimal location for surf shop.










