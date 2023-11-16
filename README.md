## Marketing Data Analysis using Statsmodels

Welcome to the repository for marketing data analysis using the powerful statsmodels library in Python. This project aims to provide insights into the relationships between marketing efforts and their corresponding sales figures, using a dataset stored in the "marketing.csv" file.

### Dataset
The "marketing.csv" file contains valuable information on various marketing scenarios, including data related to YouTube advertising efforts, Facebook advertising efforts, and newspaper advertising efforts. The dataset comprises the following columns:

- **sales**: The sales figures for different marketing scenarios.
- **youtube**: The marketing data related to YouTube advertising efforts.
- **facebook**: The marketing data related to Facebook advertising efforts.
- **newspaper**: The marketing data related to newspaper advertising efforts.

### Installation
Before running the code in this repository, ensure that you have Python installed on your system. Additionally, install the required libraries using the following command:

```bash
pip install pandas statsmodels matplotlib
```

## Code Overview

This analysis leverages the `statsmodels` library, which offers robust tools for statistical analysis in Python. The key steps in the code are as follows:

1. **Importing Required Libraries**: We start by importing the necessary libraries: `statsmodels.api` and `pandas`.

2. **Loading the Dataset**: The marketing data is read from the "marketing.csv" file using the `pd.read_csv()` function from pandas.

3. **Fitting a Simple Linear Regression**: To explore the relationship between sales and YouTube advertising efforts, we use Ordinary Least Squares (OLS) regression to fit a simple linear regression model. The results of the regression are stored in the `results` variable.

4. **Calculating Predicted Values and Residuals**: The code calculates the predicted values and residuals using the fitted model. Predicted values are stored in a new column named "Predicted" in the marketing DataFrame, and residuals are stored in a new column named "residuals".

5. **Visualizing Residuals**: We generate a scatter plot of the predicted values against the residuals, with a horizontal dashed red line representing the zero-residual line.

6. **Regression Summary**: The code performs separate regressions for sales against YouTube, Facebook, and newspaper marketing efforts. The regression summaries are printed to the console, providing insights into the coefficient estimates, p-values, R-squared values, and other relevant statistics.

7. **Scatter Plot with Regression Line**: Additionally, we create a scatter plot of YouTube against sales with a fitted regression line based on the YouTube variable.

### Running the Code

To run the code, ensure you have Python and the required libraries installed. Next, download the "marketing.csv" file and place it in the same directory as the code. Finally, execute the script as follows:

```bash
python Model_Diagnostics.py
```

### Interpretation of Results

The code provides various statistical outputs, including coefficients, p-values, and R-squared values for each regression. These values can help you interpret the relationships between marketing efforts and sales. The scatter plots visually depict the data and the fitted regression lines, aiding in understanding the linear relationships between the variables.

It is important to note that this analysis assumes a linear relationship between marketing efforts and sales figures. Interpret the results accordingly and consider other factors that may influence sales but are not present in this dataset.

### Happy analyzing!
