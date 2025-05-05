# Machine Learning Portfolio

# Linear Regression

## About the Project

### This project demonstrates how to implement Linear Regression from scratch in Python using numpy and matplotlib. It covers:

### Manual implementation of the Linear Regression algorithm

### Calculation of regression metrics (R², MSE)

### Plotting the regression line, residuals, and Q-Q plots

### Using sklearn for comparison

### Coefficient constraint handling (min/max beta)

### It includes two main components:

### MyLinearRegression class: a simple implementation of linear regression from scratch

### RegressionModel class: an extended version that includes plotting functions and constraints, plus usage of scikit-learn

## Table of Contents

* About the Project

* Getting Started

* Usage

* Visualizations

* Built With

* Results

* License

## Getting Started

## Prerequisites

### Ensure you have Python 3.x and the following libraries installed:

 pip install numpy matplotlib scikit-learn scipy

 ## Running the Code

1. Clone the repository

2. Open the Python file(s)

3. Run the examples at the bottom of the script to see results for simple and multiple regression

## Usage

## Simple Linear Regression Example

X = np.array([[1], [2], [3], [4], [5]])
y = np.array([2, 4, 5, 4, 5])
model = MyLinearRegression()
model.fit(X, y)
model.plot(X, y)

## Multiple Regression Example (using RegressionModel)

X_multi = np.random.rand(100, 2) * 100
y_multi = 3 * X_multi[:, 0] + 2 * X_multi[:, 1] + np.random.randn(100) * 10
regression_multi = RegressionModel(X_multi, y_multi)
regression_multi.fit()
regression_multi.plot_residuals()
regression_multi.plot_qq()

## Visualizations

* Scatter Plot with Regression Line

* Residual Plot

* Q-Q Plot

The plots allow you to easily diagnose model fit and check assumptions.

## Built With

 * numpy

* matplotlib

* scikit-learn

* scipy


