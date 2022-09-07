# Engine-Rating-predictions
Python script that predicts the engine rating based on the inspection parameters using only the provided dataset.

# objective 
Your task is to write a small Python that predicts the engine rating based on the inspection parameters using only the
provided dataset. You need to find all the cases/outliers where the rating has been given incorrectly as compared to
current condition of the engine.
This task is designed to test your Python ability, your knowledge of Data Science techniques, your ability to find trends,
outliers, relative importance of variables with deviation in target variable and your ability to work effectively, efficiently
and independently within a commercial setting.
This task is designed as well to test your hyper-tuning abilities or lateral thinking.

# Data
![image](https://user-images.githubusercontent.com/36518896/188848124-cf41f59f-a8a3-4ef3-b357-5f095f17c8c9.png)

# Null value in Data 
![image](https://user-images.githubusercontent.com/36518896/188848257-b2f76a43-67c4-4244-8675-f28f75d9d15b.png)

# Variable in Data 
![image](https://user-images.githubusercontent.com/36518896/188848534-732769c1-e8fa-4cc0-8b4f-d3374dc9535b.png)

# EDA of Data
![image](https://user-images.githubusercontent.com/36518896/188848698-31ba09c0-5968-4db7-b3d6-517432efcbd4.png)

# Number of inspections across dates
![image](https://user-images.githubusercontent.com/36518896/188848834-73ffd6a8-2737-4781-bbcd-15056dab299d.png)

# Performing a similar analysis across month
![image](https://user-images.githubusercontent.com/36518896/188848986-dbc8a4bc-bb41-472d-91c9-610eb98b18b3.png)

# Visualising number of inspections across Day of Month 
![image](https://user-images.githubusercontent.com/36518896/188849090-3a27c29e-deab-4b61-b22c-285522dcea42.png)

# Number of inspections across Weekday
![image](https://user-images.githubusercontent.com/36518896/188849211-e547949d-d8c4-4c1b-b6a4-b62d7815dccc.png)

![image](https://user-images.githubusercontent.com/36518896/188849297-f3a2fdea-2b38-4c80-acbe-440700a82252.png)

# Analysis of registration year
![image](https://user-images.githubusercontent.com/36518896/188849522-57412a7a-60e5-4283-8e52-42f2ba98ab20.png)

# Inspection month v/s rating_engineTransmission
![image](https://user-images.githubusercontent.com/36518896/188849710-5906776a-c189-4c01-a67c-89ddef9831a6.png)

# correlation
![image](https://user-images.githubusercontent.com/36518896/188849887-7dbadd0b-e097-4f28-8f2b-cf3126bfffb1.png)

# Final Result after putting ML model 
![image](https://user-images.githubusercontent.com/36518896/188850155-f1da4b87-0f73-4c74-b4d2-10fdb9aad706.png)



1. Briefly describe your approach to this problem and the steps you took
Ans: i have done some EDA on data set and put my analysis after each EDA.
     A. about data Description
        i. in above we see that type of inspectionStartTime column is object and it is date type column so we need to change its data type o date and time
     B. About NULL values
        i. Total number of columns which has more than 40% null values in it: 52
           52 out of 73 independent varaibles have more then 40% null values.
        ii.lest say hypothesis
           I. From the Fields_Summary, it seems that null values have to be imputed as "yes" in most of columns.
        iii. 47 out of 53 variables have a description of "current condition if not yes"
        iv.hance we can conclude that our hypothesis is true, out of 52 columns 47 column has yes as defult value so we fill the null value of all 47 columns as yes.
         v.lest check other 4 columes those has null value but condtion is other then current "condition if not yes"
        vi. As we can analyze that in above columns has more the 80% of null values and they are also not under condition of 40% more null values in it.
        vii.we have 2 options over here
                I. drop those colums
                II. We can impute "no" in above columns as mentioned in Fields_Summary
                III.it is better to drop those colums as they are not important as per above analysis
 
 # About data

total vraible data in DB including target variable : 5
Total Categorcal data in DB : 63
here we can see that out of 68 columns 64 are categorical data type and only 4 are variable data type
which means 94% data are categorical data type and only 5.8% data are varibale data type















