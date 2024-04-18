# Linear_regression
Linear Regression:
Linear regression is a statistical method used to model the relationship between two continuous variables. In this case, it's used to model the relationship between height (independent variable) and weight (dependent variable). The model assumes a linear relationship between the independent variable (height) and the dependent variable (weight), represented by the equation:
y=mx+b
where:
y is the dependent variable (weight),
x is the independent variable (height),
m is the slope of the line (coefficient),
b is the y-intercept.

The LinearRegression() model in sklearn estimates the values of m and b that best fit the data, allowing us to make predictions about the dependent variable based on new values of the independent variable.
Code Outline:

Importing Libraries:
import matplotlib
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
import sklearn
from sklearn import linear_model

This section imports necessary libraries for data visualization (matplotlib), numerical computing (numpy), data manipulation (pandas), and machine learning algorithms (sklearn).

Defining Data:
height = [[4.0], [5.0], [6.0], [7.0], [8.0], [9.0], [10.0]]
weight = [16, 25, 36, 49, 64, 81, 100]

Here, height and weight are lists representing the independent variable (height) and dependent variable (weight) respectively. Each sublist in height contains a single value.

Plotting Data:
plt.scatter(height, weight, color='black')
plt.xlabel("height")
plt.ylabel("weight")
This section creates a scatter plot using matplotlib to visualize the relationship between height and weight.

Linear Regression:
reg = linear_model.LinearRegression()
reg.fit(height, weight)
A linear regression model is created using LinearRegression() from sklearn. Then, the model is fitted to the data using fit() method, where height is the independent variable and weight is the dependent variable.

Prediction:
X_height = [[12.0]]
print(reg.predict(X_height))

This part predicts the weight for a given height (12.0) using the trained linear regression model and prints the result.









