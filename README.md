# Classification-Projects

# Will a person's salary be greater than or less than 50k
Author: Craig Gossen

## **Business problem:**
What factors drive a person's earning? This model helps classify factors to predict whether a person's earnings will be greater than of less than 50k. 

Data:
Original data set URL: https://archive.ics.uci.edu/ml/datasets/adult

## To prepare this data, the data was cleaned, and the following processes were performed:
### Exploratory Data Analysis
A basic barplot was created to determine if the dataset showed whether years of education affected salary, which one would expect. 
![image](https://user-images.githubusercontent.com/114834926/212222888-86efbea9-5a6e-4ac9-b390-a519817158d1.png)

Additionally, a heat map indicated there was minimal correlation between the numeric data columns. 

![image](https://user-images.githubusercontent.com/114834926/212223110-ac753cb7-619c-4e02-983d-0b930c684502.png)

### Explanatory Data Analysis
A lineplot was created to dive deeper into the years of schooling associated with different age groups and their salary levels. 
There was no discernable trend when looking at years of education and age. The data does show that those making >50k in salary tend to be in their core working years between the ages of 29 and 57.
![image](https://user-images.githubusercontent.com/114834926/212223446-ccd8acb0-5768-4743-bc86-11d7df913843.png)

Additionally, a countplot was utilized to show which occupations were most likely associated with the two salary levels.
![image](https://user-images.githubusercontent.com/114834926/212223689-e7883c3c-e56b-4b69-b1a2-bc98f3cc72fc.png)

### Preprocessing
Preprocessing steps included oversampling to create a balanced set of data. SimpleImputer and StandardScaler were also utilized. 

## Machine Learning Using the Following Models: Logistic Regression and K Nearest Neighbors (KNN)

### Logistic Regression
This model showed an accuracy of 78% when tuned using GridSearchCV. Additionally, PCA was applied to reduce the dimensionality with no greater results. 

### KNN
KNN showed a best accuracy of 79% accuracy with tuning and PCA being applied. KNN failed to accurately predict >50 accurately as it only could get 42% accurate. 

Overall, the best model was Logistic Regression. It appears the model is best at prediction individual's with salaries <50k vs. >50k. This suggests there are many variables which contribute to higher salaries where there are clearer paths to low salaries. 
