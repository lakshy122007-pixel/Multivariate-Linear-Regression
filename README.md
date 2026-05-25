# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>
Start the program and import the required libraries such as Pandas and Linear Regression from Scikit-learn.
### Step2
<br>
Read the CSV file and store the input features (Weight, Volume) and target value (CO2).

### Step3
<br>
Train the Linear Regression model using the given dataset and calculate coefficients and intercept.

### Step4
<br>
Predict the CO2 emission for the given Weight and Volume values and display the result.

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2
```
## Output:

### Insert your output
<img width="1538" height="453" alt="image" src="https://github.com/user-attachments/assets/eb4bc80a-7957-4bab-9833-65c318ebf92e" />

## Result:
Thus the multivariate linear regression is implemented and predicted the output using python program.
