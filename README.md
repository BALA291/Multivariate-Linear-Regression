# EX.NO-10 Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd.

### Step2
Read the csv file.

### Step3
Get the value of X and Y variables.

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of the car where the weight is 2300kg,and volume is 1300cm cube.

### Step6
Print the predicted output.

## Program:
```
# NAME : BALAMURUGAN B
# REG NO :212222230016
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("/content/cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted Co2 for the corresponding weight and volume",predictedCO2)

```
## Output:
![mai 10](https://github.com/BALA291/Multivariate-Linear-Regression/assets/120717501/7c460104-263b-46a2-89d3-c1a7b61131ec)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
