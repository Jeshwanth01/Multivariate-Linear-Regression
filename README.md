# DATE :-
# EXP 10: Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## step 1 Load the dataset.
Handle missing values and encode categorical variables.
Split the data into training and testing sets.
## step 2 Feature Selection

Identify the independent variables (features) and the dependent variable (target).
Prepare the data matrices for features (X) and target (y).
## step 3 Model Training

Import the LinearRegression model from sklearn.linear_model.
Train the model using the training data (X_train and y_train).
## step 4 Prediction

Use the trained model to predict the target values for the testing set (X_test).
## step 5 Evaluation

Evaluate the model’s performance using metrics like Mean Squared Error (MSE) and R-squared.
Optionally, visualize the results by plotting actual vs. predicted values.
 
## Program:
```
#program devoleped by - JESHWANTHR 
#registration number - 2305003003
#Write a python program to implement univariate Linear Regression to fit a straight line using
import pandas as pd
from sklearn import linear_model
data=pd.read_csv("/content/car.csv")
x=data[['Weight','Volume']]
y=data[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficiants:',regr.coef_)
print('Intercept:',regr.intercept_)
predictCO2=regr.predict([[3300,1300]])
print('predicted CO2 for the corresponding wieght and volume',predictCO2)





```
## Output:
![EXP 10 MAI](https://github.com/Jeshwanth01/Multivariate-Linear-Regression/assets/145525167/4899b0fe-f805-4584-8073-986f8dadd608)



<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
