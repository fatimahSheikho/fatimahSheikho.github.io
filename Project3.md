
# Predicting Crimes Categories in Denver City
# Purpose 
The main purpose of my model is to predict type of the crimes to help prevent recurring crimes in an area as well as identifying the most common types of crime in the area.
# Dataset Parameters:
381K rows 8 features 
# Features:
## Location
- Precinct ID
- Incident Address
- Longitude
- Lattitude
## Date
- Crime occurrence date
- Last occurrence date
- Diffrence in hours between reported and occurrence date
## Offense 
- Offense code extension
# Workflow
## Data Acquisition 
I acquired the data from [Denver City and County ](https://www.denvergov.org/opendata/dataset/city-and-county-of-denver-crime). 
## EDA
To gain more insight about my categories and to know more about the occurrence of each per year. 
## Data Cleaning 
1- Reduced the number of categories from 15 to 6.
2- Dropped all traffic accidents rows.
3- Filled NaNs.
4- Splitt dates into hour/day/month/year. 
## Baseline
I split off my data into training, validation and testing. Then, I created my baseline model using KNN R^2=0.62.
## Feature Engineering 
My classes were not balanced to fix this I applyed the SMOTE technique.

## Model Training and Validation
I trained and validated on the following models:

- Random Forest Classifier
Accuracy: 0.84
F1: 0.78
- Logistic Regression  
Accuracy: 0.63
F1: 0.28
- SVC
Accuracy: 0.43
F1: 0.27

- Naive Bayes 
Accuracy: 0.77
F1: 0.63

## Testing 
Tested on best performed model which is Random Forest Classifier. And the results were 
Accuracy: 0.82
F1: 0.78.

## Conclusion:
With the number of insights gained from data, police officers can understand in what areas they would need more training or a change in policies for effective crime prevention.




