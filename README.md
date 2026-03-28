# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas ass pd.

### Step2
Read the CSV File.

### Step3
Get Values of X and Y variable.

### Step4
Create teh linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.

## Program:
```
# Developed BY:madhesh V
# Reg No:212225040214


import pandas as pd
from sklearn import linear_model
df = pd.read_csv("car.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
predictedCO2 = regr.predict(pd.DataFrame([[3300, 1300]], columns=['Weight', 'Volume']))
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)


```
## Output:
<img width="615" height="62" alt="526965218-efb31b40-16a0-4123-8cbd-f6d555f0b12b" src="https://github.com/user-attachments/assets/1bfcea5c-2ea4-4e8b-a755-c2856ec31717" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
