# nyc-crashes : Information about the repository #

> ### Documents Information ###

* **original_data_100000.csv file**

You will find here the original dataset i started to work with.

* **cleaned_data_100000.csv file**
> Work in progress

You will find here the final .csv file with the cleaned dataset. 

* **extremely_simplified_data_100000.csv file**

You will find here a mini version of the dataset in a .csv file, containing info on the streets and on the amount of people killed or injured.

* **NYC_Crashes_Source_Code.ipynb file**

You will find here the source code that i wrote to be able to clean the original dataset and create the final **cleaned_data_100000.csv** file (see here above).

Libraries that i used : 

### Project Mission ###

Bill de Blasio, mayor of New York City, is in a bit of a pickle. Indeed, his police department, the NYPD, collected information about all the traffic accidents that happened in New York City. However, they are too busy eating doughnuts to correctly encode each traffic indicent, and so it happens that the dataset that we got here is quite dirty, has a lot of missing values and can't be used by a machine learning model as is. Can you help Mr. de Blasio and shine a new light on his police department ?

:collision:  **What he wants exactly is to predict which streets are the most dangerous while visiting the city that never sleeps.**  :collision:

### Dataset explained ###
> Sometime it can be confusing in what does each variable translate in real life and thus what does it mean. 
> This is important to understand to be able to make sense of the data, and later on to know what decision to take in term of cleaning and preprocessing that allow us to keep a meaningful data while making it ready to work.

Information concerning the dataset is well explained and can be find on the website of New York City (see the link below)

[NYC website source](https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95)



### Work-flow ###

#### :rocket: First step : Get and understand the dataset

Importing required Libraries (ex:Pandas)
Creating a dataframe out of the original .csv file
First check of the dataset and understanding the different variables and values (see here above **Dataset explained**)


#### :rocket: Second step : Start of the cleaning

* **1 / Check out for missing values : .isnull().sum() functions**

It gives us an understanding and a vision on where are the missing values, in which columns.
We can then ask ourselves some questions such as : 
Is this column really relevant or meaningful? 
Can I, Should I drop it?
Can I find a way to fill the missing values?

* **2 / Check the unique values of each columns : .unique()** 

Checking the unique values in each columns allow me to compare some columns between eachother. 
Aswell it can highlights the redundancy of a term written in different way, and therefore that could be object to consolidation by harmonizing all the different spelling as one
By exemple : [tow truck, Tow Truck, TOW TRUCK, tow Truck, Tow truck] , this 5 items from that list represent the same type of truck and therefore we could adapt their spelling resulting, for example, in having only [Tow Truck] left as unique value

* **3 / Reducing the amount of column**
Here, after I noticed that some columns were missing values, i also noticed that for our purpose we could easily reduce the amount of columns in our dataset without losing the meaning of it. 
By exemple: the 5 different vehicules columns could be put in one

To do so I created a new column gathering the values of the different columns i wanted and could 'merge' together.
For the 'street_name' newly created column, gathering the 3 other column concerning the street name where the accident occured, I had first to remove the different 'NaN' values that i repaced with empty strings ("") 



* **4/ Consolidation**

* **5/ Duplicates**

#### :rocket: Third step : Implement some features


### Choices Explained ###

### State of the project ###

**Must have features** 

**Nice-to-have features**
