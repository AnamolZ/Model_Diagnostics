Marketing Data Analysis using Statsmodels
This repository contains code to analyze marketing data using the statsmodels library in Python. The dataset used in this analysis is stored in the "marketing.csv" file.

Dataset
The "marketing.csv" file contains a dataset with information on marketing efforts and their corresponding sales figures. The columns in the dataset are as follows:

sales: The sales figures for different marketing scenarios.
youtube: The marketing data related to YouTube advertising efforts.
facebook: The marketing data related to Facebook advertising efforts.
newspaper: The marketing data related to newspaper advertising efforts.
Installation
To run the code in this repository, you need to have Python installed on your system. Additionally, make sure to install the required libraries using the following command:

bash
Copy code
pip install pandas statsmodels matplotlib
Code Overview
The analysis is performed using the statsmodels library, which provides powerful tools for statistical analysis in Python. Below is an overview of the key steps in the code:

Importing Required Libraries: The code begins by importing the necessary libraries: statsmodels.api and pandas.

Loading the Dataset: The marketing data is read from the "marketing.csv" file using the pd.read_csv() function from pandas.

Fitting a Simple Linear Regression: The code uses Ordinary Least Squares (OLS) regression to fit a simple linear regression model with sales as the dependent variable and youtube as the independent variable. The results of the regression are stored in the results variable.

Calculating Predicted Values and Residuals: The predicted values and residuals are calculated using the fitted model. The predicted values are stored in a new column named "Predicted" in the marketing DataFrame, and the residuals are stored in a new column named "residuals".

Visualizing Residuals: The code generates a scatter plot of the predicted values against the residuals. The horizontal dashed red line represents the zero-residual line.

Regression Summary: The code performs separate regressions for sales against youtube, facebook, and newspaper. The regression summaries are printed to the console, providing insights into the coefficient estimates, p-values, R-squared values, and other relevant statistics.

Scatter Plot with Regression Line: The code creates a scatter plot of youtube against sales with a fitted regression line based on the youtube variable.

Running the Code
To run the code, make sure you have Python and the required libraries installed. Then, download the "marketing.csv" file and place it in the same directory as the code. After that, simply execute the script.

bash
Copy code
python your_script.py
Interpretation of Results
The code provides various statistical outputs, including the coefficients, p-values, and R-squared values for each regression. These values can be used to interpret the relationships between marketing efforts and sales. Additionally, the scatter plots visualize the data and the fitted regression lines, helping to understand the linear relationships between the variables.

Please note that this analysis assumes a linear relationship between the marketing efforts and sales figures. It's essential to interpret the results within this context and consider other factors that may influence sales but are not included in this dataset.

License
This code is provided under the MIT License. Feel free to use, modify, and distribute the code according to the terms of the license.
