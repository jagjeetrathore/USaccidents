# USaccidents Pyspark Project

US-Accidents: A Countrywide Traffic Accident Dataset - Sobhan Moosavi
This is a countrywide motor-vehicle crash dataset, which covers 49 states of the United States. The data is continuously being collected from February 2016. Currently, there
are 3.5 million accident records in this dataset. Each accident record is described by a variety of attributes including location, time, weather, and nearby points-of-interest.
smoosavi.org


#### Objectives 
First Objective of this project was to do exploratory analysis of US Accidents data to determine if external factors like weather precipitation or other environmental stimuli 
incorporated in the accident's volume or severity. Second Objective was to create machine learning models to do real time predictions., using custom machine learning models.
I have attempted to solve this problem using two machine learning models: Random Forest and Logistic Regression.
This type of analysis can help traffic control departments to focus on right factors to address or control, in order to lower down the severity and/or number of accidents
overall.

### Challenges: 
Major challenges that we faced before performing analysis and modelling were the data cleansing i.e. taking care of nulls, standardizing data values and data prep i.e.
converting categorical values to numeric for modelling that was done using String Indexer.
We took care of nulls by dropping columns with more than ~ 50% of missing data, using mode and/or median values to fill in missing data rows for some important numeric fields.
Also, we dropped rows for text fields where we were not able to fill in data for those rows and this kind of columns had low number of nulls hence dropping such rows did not 
highly impact the volume of data.

### Exploratory Data Analysis:
Heatmap, Visualization Tools/Libraries Matplotlib, Seaborn and Databricks 

### Predictive Models :
Random Forest Classifier and Logistic Regression algorithms to try to predict the severity of accidents based on relevant features in the dataset.These algorithms were chosen 
for their versatility when applied to a wide range of data set types. 

### Conclusions: 
It was clear from the analysis that most accidents happened during day time and road barriers or traffic signals played little to no role in severity or volume of accidents.
Most of the accidents happened when the weather was calm which point towards our hypothesis that the majority of accidents happened due to human factors only like careless
or rash driving.


The Random Forest Classifier outperformed Logistic Regression and was able to predict the severity over 70% of the time.
 
In the future, I also can group the dataset into two groups of severities and turn this into a binary classification problem since there are 99.69% accidents from severity 2
and 3. It could improve the accuracy of the models.
