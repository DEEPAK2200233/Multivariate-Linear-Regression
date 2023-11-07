## Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.

## Equipment’s required:
Hardware – PCs
Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step2: Read the csv file.

Step3: Get the value of X and y variables.

Step4: Create the linear regression model and fit.

Step5: Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.

Step6: Print the predicted output.

## Program:
```
Developed by: DEEPAK RAJ S
Reg.No: 212222240023

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars (1).csv")
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient: ",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("predicted CO2 for the corresponding weight and volume",predictedCO2)

```
## Output:
![image](https://github.com/DEEPAK2200233/Multivariate-Linear-Regression/assets/118707676/702e8690-4d93-4657-a8db-06df3914e6f1)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
