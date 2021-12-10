# automobile_capstone

README: Capstone II

Automobile Exploratory Data Anaylsis

Our code in Jupyter Notebook performs the following steps:
1.	Preview data
2.	Check total number of entries and column types
3.	Check any null values
4.	Check duplicate entries
5.	Plot distribution of numeric data (univariate and pairwise joint distribution)
6.	Analyse time series of numeric data by price frequencies

Keeping in mind that the problem statement is to forecast the dealership sales, our EDA objectives are, therefore:
1.	To check for features that can help in forecasting sales; and
2.	To check for anomalies or outliers that may impact our forecasting model

The output shows that we have around 205 entries with 26 columns initially. 
No null values but some of the columns’ data type should be changed. 
As we shall see later, setting the data types correctly can aid us in our data science processes. 
In a nutshell, there are three common types of data type (categorical, numeric and date-time) and 
we have different EDA procedures for each of them. But in our case we don’t have the date-time data type.
In our preliminary processing, we changed the data types in the following way:
•	Set the identifier Make as string, well in our case an object is already a string.
•	For columns that are categorical, i.e., columns that take on a limited, 
    and usually fixed, number of possible values, we set their type as “category”. 
	E.g., fuel-type, engine-location, body-style, etc. are all categorical data.
•	For columns that are numeric, we can either set their type as “int64” (integer) or “float64” (floating point number). 
    E.g., engine-size, weight and price are all numeric data.


WE BEGIN WITH DATA CLEANING

After setting the data types, and previewed the dataset, we begin with EDA.
And it’s that’s very Simple :) 
Let’s now go through the salient parts of the output to understand how to make use of our EDA results.

Missing values and Duplicated Entries
In our case, there is no entry with missing values.
However, in the event of missing values, the code will generate a chart similar to the one in Automobile.ipynd(Juypter Notebook). 
Notice the white spaces under CustomerID and Description; those are the missing values. 
Thus, in one glance, we are able to know the extent of our missing values issue.

Numeric Data EDA
On our code we have sorted the price column by ascending order and removed entries which did not have a valid price. 
In our case we had entries which included “?” on the price column, that too is part of Data Cleaning process.

We also saw the Pie chart come into play.

Lastly, do note that depending on our data science problem statement, we may wish to perform additional EDA steps. 
Nonetheless, the code template should be able to cover the basic EDA and get us up to speed quickly.
