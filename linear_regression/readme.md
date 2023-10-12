# Linear Regression

This repository contains code for simple linear regression in Python. The code uses numpy and matplotlib for numerical computations and visualization, and pandas for data manipulation.

## Overview

The code demonstrates simple linear regression using randomly generated data. It follows these steps:

1. Generate random data points `x` and `y` with added noise.
2. Plot the generated data.
3. Fit the data using linear regression to find the parameters `theta0` and `theta1`.
4. Plot the true regression line and the estimated regression line.
5. Calculate the coefficient of determination ($R^2$) to measure goodness of fit.

## Theory

### Linear Regression Model

The linear regression model is given by:

$$\hat{y} = \theta_0 + \theta_1 x$$

Where:
- $\hat{y}$ is the predicted value.
- $\theta_0$ is the intercept.
- $\theta_1$ is the slope.

### Parameter Estimation

The parameters $\theta_0$ and $\theta_1$ can be estimated using the following formulas:

$$\theta_1 = \frac{\sum_{i}^{n} (x_i-\overline{x})(y_i - \overline{y})}{\sum_{i}^n(x_i - \overline{x})^2 } = \frac{\overline{xy} - (\overline{x})(\overline{y})} {\overline{x^2} - (\overline{x})^2}$$

$$\theta_0 = \overline{y} - \theta_1 \overline{x} = \frac{(\overline{x^2})(\overline{y}) - (\overline{x})(\overline{xy})}{\overline{x^2} - (\overline{x})^2}$$

### Coefficient of Determination ($R^2$)

The coefficient of determination is a measure of goodness of fit. It is defined as:

$$R^2 = 1 - \frac{\textrm{SSR}}{\textrm{TSS}} = 1 - \frac{\sum_i \left(y - \hat{y}_i\right)^2}{\sum_i \left(y - \bar{y}\right)^2}$$

where:
- SSR is the sum of squared residuals.
- TSS is the total sum of squares.

$R^2$ is unitless and ranges from 0 to 1. A higher $R^2$ indicates a better fit.

## Usage

To use this code, simply run the provided Python script. The generated plots will illustrate the steps of linear regression.

For more detailed information on linear regression, you can follow this [link](https://en.wikipedia.org/wiki/Linear_regression).

For any questions or further assistance, please don't hesitate to reach out.
