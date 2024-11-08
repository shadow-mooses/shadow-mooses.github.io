### Repository for Activities 9.1 and 9.2

### Shadow Mooses portfolio
### Introduction
The MIT class knowledge journey has brought me very far. From basic python coding, to applied mathematics like statistics and linear regression to creating a programmatic process for uploading data to a mySQL database.

Here are some of the projects I've worked on thus far.


#### Table of contents

- [linear regression](#item-one)
- [ETL from csv to mysql database](#item-two)
- [plotting fermenation progress](#item-three)

<!-- headings -->

<a id='item-one'></a>
### Linear regression modelling 

#### Overview
For this project we were given a dataset of housing prices with qualitative and quantitative attributes to build a predictive model of housing prices. We used libraries like matplotlib, pandas, numpy and sklearn to build our model.

#### Python Libraries
Pandas, SKLearn, Numpy, Matplotlib.

#### Data
The trained data was a table of housing prices with dozens of attributes to describe the houses in qualitative and quantitiative values. Some of the values were ranged, (1-10) or there were indexed by letters (P,F,G,E). Overall, this data was relatively clean and we were given a data glossary to assist with the initial analysis. The data was given in csv form and we imported it and converted it into a dataframe. 

#### Process
We began by importing data, cleaning it, removing NaN values and skewed values and chose the attributes that had the best correleation coefficient for our X values or indpepndant variables. The house sale price would be our Y value or our dependant variable. The data 

Then we built our model with those attributes to find our slope values and r^2 value, our goal was to create a model with >0.83 fit with our trained data.

Then we used sample data and found that our model had a ~0.72 fit.

<a id='item-two'></a>
### ETL - Static csv to MySQL database

#### Overview
I was very excited for this project since it has many real world applications and is one of the main functions of a data engineer (in my opinion). We were tasked with taking a dataset in excel and importing it into mysql.

#### Python Libraries
Pandas, MySQL connector, Matplotlib, Yaml

#### The data
We were given an excel sheet with sheets that were each year from 2011 to 2022. Each sheet had the same headers and columns and formatting but required lots of cleaning and reformatting before it could be imported. It also provided good practice with formatting data correctly before importing into a sql database (removing special characters, formatting integers and strings, etc.)

#### The process
First, we configured our mysql connector and database connection. Then cleaned our dataset. After cleaning the data, creating our ERD diagram to outline how we wanted the data to be imported. We created our import scripts in python to create the database and the tables. 

Then we configured our cursor and looped over lines in our csv with a sql query and executed the cursor to create and commit new values to each table.

Once our tables were complete, we then wrote queries in python and sql to learn more about our dataset. We combined the rich library of python libraries and graphs to plot data.

#### The result
We were able to programmatically read data in csv/excel form, connect to a database, write import scripts, extract data, tansform it and load it into our database. Then query using python and conver to a dataframe.

<a id='item-one'></a>
### Plotting fermenation process

#### Overview
In my spare time, I brew my own beer and while humans have been brewing for thousands of years, there is a ton of science involved and lots that we don't know.

One key indicator of the process of fermentation (yeast synthesising sugar into CO2) is measuring the amount of dissolved sugar in solution in real-time along with temperature.

This is done with an accelerometer sensor that is able to feed several datapoints back to a cloud database (google sheet or website). It is valuable and useful data to practice with since it includes, floats, strings and datetime values.

#### The Process
TK 