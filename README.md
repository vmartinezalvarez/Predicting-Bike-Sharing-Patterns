![Center Image](images/fig1.jpg)

# Predicting Bike Sharing Patterns in Colab
Bike sharing systems are new generation of traditional bike rentals where whole process from membership, rental and return 
back has become automatic. Through these systems, user is able to easily rent a bike from a particular position and return 
back at another position. Currently, there are about over 500 bike-sharing programs around the world which is composed of 
over 500 thousands bicycles. Today, there exists great interest in these systems due to their important role in traffic, 
environmental and health issues. 

Apart from interesting real world applications of bike sharing systems, the characteristics of data being generated by
these systems make them attractive for the research. Opposed to other transport services such as bus or subway, the duration
of travel, departure and arrival position is explicitly recorded in these systems. This feature turns bike sharing system into a virtual sensor network that can be used for sensing mobility in the city. Hence, it is expected that most of important
events in the city could be detected via monitoring these data.

## About the Data Set
Bike-sharing rental process is highly correlated to the environmental and seasonal settings. For instance, weather conditions, precipitation, day of week, season, hour of the day, etc. can affect the rental behaviors. The core data set is related to the two-year historical log corresponding to years 2011 and 2012 from Capital Bikeshare system, Washington D.C., USA which is publicly available in http://capitalbikeshare.com/system-data. They have aggregated the data on two hourly and daily basis and then extracted and added the corresponding weather and seasonal information. Weather information are extracted from http://www.freemeteo.com.

### Dataset characteristics
	
Both hour.csv and day.csv have the following fields, except hr which is not available in day.csv
	
	- instant: record index
	- dteday : date
	- season : season (1:springer, 2:summer, 3:fall, 4:winter)
	- yr : year (0: 2011, 1:2012)
	- mnth : month ( 1 to 12)
	- hr : hour (0 to 23)
	- holiday : weather day is holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
	- weekday : day of the week
	- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
	+ weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
	- temp : Normalized temperature in Celsius. The values are divided to 41 (max)
	- atemp: Normalized feeling temperature in Celsius. The values are divided to 50 (max)
	- hum: Normalized humidity. The values are divided to 100 (max)
	- windspeed: Normalized wind speed. The values are divided to 67 (max)
	- casual: count of casual users
	- registered: count of registered users
	- cnt: count of total rental bikes including both casual and registered

## Project Description

Predict the number of bikeshare users on a given day using a neural network built from scratch, and using tensorflow.

In this project, I build a neural network from scratch to carry out a prediction problem on a real dataset! By building a neural network from the ground up, you'll have a much better understanding of gradient descent, backpropagation, and other concepts that are important to know before we move to higher level tools such as Tensorflow. You'll also get to see how to apply these networks to solve real prediction problems!

## Table Of Contents
* [Data Set](https://github.com/vmartinezalvarez/Predicting-Bike-Sharing-Patterns/blob/master/Bike-Sharing-Dataset)
	- [hour.csv](https://github.com/vmartinezalvarez/Predicting-Bike-Sharing-Patterns/blob/master/Bike-Sharing-Dataset/day.csv) : bike sharing counts aggregated on hourly basis. Records: 17379 hours
 	- [day.csv](https://github.com/vmartinezalvarez/Predicting-Bike-Sharing-Patterns/blob/master/Bike-Sharing-Dataset/day.csv) : bike sharing counts aggregated on daily basis. Records: 731 days
* [Neural_networks_from_scratch_Predicting_Bike-Sharing_Patterns.ipynb](https://github.com/vmartinezalvarez/Predicting-Bike-Sharing-Patterns/blob/master/Neural_networks_in_TensorFlow_Predicting_Bike_Sharing_Patterns.ipynb): Building a neural network from scratch in [Colab](https://colab.research.google.com) to predict bike-sharing patterns.
* [Neural networks in TensorFlow. Predicting Bike-Sharing Patterns.ipynb](https://github.com/vmartinezalvarez/Predicting-Bike-Sharing-Patterns/blob/master/Neural_networks_in_TensorFlow_Predicting_Bike_Sharing_Patterns.ipynb): Building a neural network in [Colab](https://colab.research.google.com) using [TensorFlow](https://www.tensorflow.org/) Low Level API to predict bike-sharing patterns. Save and restore variables and models.

## Quick Start

You can open the notebooks directly in [Colab](https://colab.research.google.com), which is a free Jupyter notebook environment that requires no setup and runs entirely in the cloud, and provides a free GPU or TPU services. Also you can download the project materials from this GitHub repository. You can get clone the repository  to your computer with ``git clone https://github.com/vmartinezalvarez/Predicting-Bike-Sharing-Patterns.git``.

## Related Task

- Regression: Predication of bike rental count hourly or daily based on the environmental and seasonal settings.
- Event and Anomaly Detection: Count of rented bikes are also correlated to some events in the town which easily are traceable via search engines.

## References
- Udacity Deep Learning Nanodegree: Predicting-Bike-Sharing-Patterns.
- Fanaee-T, Hadi, and Gama, Joao, "Event labeling combining ensemble detectors and background knowledge", Progress in Artificial Intelligence (2013): pp. 1-15, Springer Berlin Heidelberg, doi:10.1007/s13748-013-0040-3.





	




