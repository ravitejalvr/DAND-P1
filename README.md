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

## Conclusion

### Limitations

The following are some of the limitations of the data given, hence the conclusions drawn from it.

As shown in IPython notebook attached, 9 columns of data are given to work with, essentially three of them being irrelevant. Additionally, there were only 891 rows of data, of which 179 were missing important fields such as age. Having some more features on the Passengers such as bodyweight (crucial since the lifeboats are space-crunch), race & reason for death (starving / lack of life boats) can be really helpful in further understanding of the disaster. 

Also, details for various columns and reasons for diving them is not given. For example, Pclass is given but it was not mentioned whats the basis. In titanic, we know there were many different classes based on fare. So, if the class is not dependent on fare, reason for its division needs to be given. 

Also, if the area of ship which sank first and cabin location of the passengers closeby is given, it would've led to better interpretation of given cabin column.

The impact of various factors is discussed below:

### Class

Probably, the strongest indicator for survival is Class. It was clearly observed that people from 1class has almost twice survival rates when compared second and third class.

### Gender

As expected, males had less chance of survival rate than women. Its observed that 63.1% of total survived people were females and only 35.2% of total people were females. Females had a survival rate of 74.2%. these numbers prove that Females of al had a much highre chance to survival than men of all ages. 

### Age

As we have seen in plots and analysis, Age is not a huge factor in deciding the survival of a person. This was interesting given that people assume children and older people will be rescued first. 

### Final Conclusion

In conclusion, the strongest evidences for survival are socioeconomic class & Gender. Passenger classis first important reason for survival. Since location and details about the clas were not given, we can discuss more about what is the issue. 

Gender also played a close second. "Women and children" was certainly a phrase that nicely sums up this gender discrepancy. However, Age didn't have any impact with regards to a passenger's survival, which is surprising. This can be the reason that data is biased and not representing total picture but a subsection of it. Since details of total number of passengers and how this data is selected from the master data is not given, we cannot make concrete conclusions but only inferences which can/cannot be true.
