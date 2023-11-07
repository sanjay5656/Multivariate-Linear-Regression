# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1:  Read the csv file.
### Step2: Get the value of X and y variables.
### Step3: Create the linear regression model and fit.
### Step4: Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.
### Step5: Print the predicted output.

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("/content/cars_(1).csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:", regr.coef_)
print("Intercept:", regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predictedd co2 for the corresponding weight and volume", predictedCO2)
```
## Output:

### Insert your output

![image](https://github.com/sanjay5656/Multivariate-Linear-Regression/assets/115128955/29743734-96d5-481c-b4c1-b340b0a686e3)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
