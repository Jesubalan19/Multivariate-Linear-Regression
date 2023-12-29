# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas.

### Step2
Import linear model from sklearn.

### Step3
Read the files cars.csv.

### Step4
Assign the values for x and y as required.

### Step5
Create the LinearRegression model and Predict the output

## Program:
```
Developed by: Jesubalan A
RegisterNumber: 23013427

import pandas as pd
from sklearn import linear_model
df=pd.read_csv('cars.csv')
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for the corresponding weight and volume",predictedCO2)

```
## Output:
![Ex 10](https://github.com/Jesubalan19/Multivariate-Linear-Regression/assets/144979294/26a611d4-12b4-4224-8932-c26e89d3b042)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
