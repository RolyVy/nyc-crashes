# nyc-crashes : Information about the repository #

> ### Documents Information ###

* **original_data_100000.csv file**

You will find here the original dataset i started to work with.

* **cleaned_data_100000.csv file**

You will find here the final .csv file with the cleaned dataset. 

* **Source code file**

You will find here the source code that i wrote to be able to clean the original dataset and create the final **cleaned_data_100000.csv** file (see here above).

Libraries that i used : 

### Project Mission ###

### Dataset explained ###
> Sometime it can be confusing in what does each variable translate in real life and thus what does it mean. 
> This is important to understand to be able to make sense of the data, and later on to know what decision to take in term of cleaning and preprocessing that allow us to keep a meaningful data while making it ready to work.

Information concerning the dataset is well explained and can be find on the website of New York City (see the link below)

[NYC website source](https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95)



### Work-flow ###

First step : Get and understand the dataset

Importing required Libraries (ex:Pandas)
Creating a dataframe out of the original .csv file
First check of the dataset and understanding the different variables and values (see here above **Dataset explained**)


Second step : Start of the cleaning

1 / Check out for missing values : .isnull().sum() functions

It gives us an understanding and a vision on where are the missing values, in which columns.
We can then ask ourselves some questions such as : 
Is this column really relevant or meaningful? 
Can I, Should I drop it?
Can I find a way to fill the missing values?

2 / Check the unique values of each columns : .unique() 

Checking the unique values in each columns allow me to compare some columns between eachother. 
Aswell it can highlights the redundancy of a term written in different way, and therefore that could be object to consolidation by harmonizing all the different spelling as one
By exemple : [tow truck, Tow Truck, TOW TRUCK, tow Truck, Tow truck] , this 5 items from that list represent the same type of truck and therefore we could adapt their spelling resulting, for example, in having only [Tow Truck] left as unique value

3 / Reducing the amount of column
Here, after I noticed that some columns were missing values, i also noticed that for our purpose we could easily reduce the amount of columns in our dataset without losing the meaning of it. 
By exemple: the 5 different vehicules columns could be put in one



4/ Consolidation

5/ 

### Choices Explained ###

### State of the project ###

**Must have features** 

**Nice-to-have features**
