# Welcome to My Ds Babel
***

## Task
The task is to build 2 functions to convert csv data to sql and sql to csv. 

## Description
To convert sql table data to csv, I have created the function which connects to a database,
reads the columns, and copies the column elements into a csv string. 
To convert csv data to sql string, I have created the function which reads the csv file, stores the 
data in a list, connects to a database, creates the desired table, and copies the list elements into
the table

## Installation
You can run the program by using python my_ds_babel.py

## Usage
After being executed, the program will run the function sql_to_csv, which converts sql table data to csv 
string. The function will connect to the database given as a parameter and fetches the table content as a
list of tuples, each of which contains column elements. 
After that, the program will try to convert all column elements to strings in order to join them together. 
In the end, the function will return the csv string. 

When the function terminates, the program will open the 'list_volcano.csv' file and pass the resulting 
object to the function csv_to_sql, which converts csv data to sql table data. At that point, the function 
will read the file and prepare the list rows_and_columns, which will store tuples, which in turn store column
elements. After that, the program will analyze each column element and convert string ints to ints and string 
floats to floats. 
In order to create a table, the program will need to use 'CREATE TABLE' query with specific table name and columns. 
To find out the number of columns and their types, the program will iterate through a sample row and obtain their 
types in SQL format. Having done so, the program will pass the commands to the cursor. 

### The Core Team
Galymzhan Zharas

<span><i>Made at <a href='https://qwasar.io'>Qwasar Silicon Valley</a></i></span>
<span><img alt='Qwasar Silicon Valley Logo' src='https://storage.googleapis.com/qwasar-public/qwasar-logo_50x50.png' width='20px'></span>
