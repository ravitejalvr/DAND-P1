# Data Analyst Nano Degree Project-1:

## Introduction:

This project objective statement is to explore a dataset of choice.

I selected Titanic Dataset. It has the data of the people who survived and not survived the crash in a .csv format. Also, various columns which give the detail of the passengers is given in the data. This dataset is subjected to various analyses to find patterns in people who survived the crash and people who did not.

## Data Wrangling:

The DataSet contained 891 rows and 9 columns. It had missing values in Age, Cabin and Embarked. However, for embarked the missing values are less and can be ignored. For age I filled it with zero as I am not sure what category of age is missing and I can always use 0 as separate category and do analysis. The graphs generated were part of the html and ipython notebook in this repository.

It is observed that 342 people out of 891 people survived. Various analysis for identifying survival is done.
Firstly, the data is imported and seen for missing values. It is observed that Age and Cabin are having maximum missing values. Age is having about 177 missing values and Cabin is having over 680 missing values.

Cabin is ignored from future analysis as it is having major data missing.

## Analysis of Data - Questions asked:
1. What are chances of survival if Age > 40
2. What are chances of survival if Embarked = Q
3. What are chances of survival if Fare > 70.

1.30.67%. The details of implementation are found in IPython Notebook. I just used pandas.groupby function for finding out this answer

2.63.82%. It is implemented in a similar fashion as question-1.

3.72.3%. Implementation is similar to questions 1 & 2.

## Data Exploration:

Bunch of charts were generated to explore and understand the data.

Three histograms were plotted for Passenger Class, Fare and Age.

By looking at Passenger Class histogram, it can be understood that Passenger Class-3 people had less chance of survival.
Observing Fare Histogram, it cna be observed that people with fare>70 had a good survival rate when compared to other fare ranges4
From Age Histogram, it can be concluded that all ages suffered equally but people of age group 0-10 had slighly better chance of survival.

Two boxplots were generated for Age and Fare and it can be seen that the distribution of Age for survived and not survived is nearly same indicating age is not a serious criterion to differentiate survivals.

Also, a histogram combining Sex and Passenger Class is generated and it is seen that females from 1st and second class had a really high chance of survival rates (>92%) and males from classes 2 & 3 has <20% survival rates.

## Conclusion:

It can be understood that females who are from higher classes were rescued first. Also, age is not clearly a barrier and the distinguishing feature is Passenger Class and Fare. Also, place of embark is having a slight impact and people who embarked from Q had slighly better survival rates.

The above conclusions made are only based on less data available. (<30%) If total data is analyzed, we might find key insights on survival rate. Particularly the Age not being a crucial factor is of particular interest. 

Even for predicting the survival rate, the current data is not sufficient for training the Machine Learning / Neural Network model.

Also, the ecenomic class of the people in the ship is not mentioned which might be a differentiating factor. 

The missing values for Age are filled with zero instead of mean value and ommitting as I thought we can analyze the missing age valuesas well without messing with other bins and ommitting them. I found that missing age values are having less than mean survival rates. Also, going by the trend in the data, it can be possible that missing age values are from higher value bins.

It is observed that with increase in fare, survival rate increase, increase in age decreased survival rate & finally
people from class 1 & 2 have more than twice survival rate than people from class 3.

Also, a chi-squared analysis for Age, Fare & P-class is done for understanding the distribution. It is observed that Both Age and Fare had higher statistic and zero p-values. And, Pclass had much lesser statistic and a p-value of 1.

These are some of my observations from Titanic Data-Set. For plots and implementation, please visit IPython Notebook.
