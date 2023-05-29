# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
find the mean of x and y.

### Step2
 calculate the slope
### Step3
apply linear regression and find the coefficient and intercept.

### Step4
plot the scattered plots

### Step5
draw the best fit line

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("/content/cars (1).csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intersept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO2 :",predictedCO2)
```
## Output:
Coefficient: [0.00755095 0.00780526]
Intersept: 79.69471929115939
Predicted CO2 : [114.75968007]
/usr/local/lib/python3.10/dist-packages/sklearn/base.py:439: UserWarning: X does not have valid feature names, but LinearRegression was fitted with feature names
  warnings.warn(

### Insert your output
![Screenshot 2023-05-29 140844](https://github.com/shalinikannan23/Multivariate-Linear-Regression/assets/118656529/b12280ed-a3b2-4930-8659-c6725c8092ee)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
