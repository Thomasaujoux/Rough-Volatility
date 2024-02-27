# Rough-Volatility

This project focuses on analyzing the volatility of financial markets using Python. It leverages popular libraries such as Pandas, NumPy, SciPy, scikit-learn, Matplotlib, and Statsmodels to process and analyze financial data, specifically looking into the realized volatility indices. The core functionality revolves around data manipulation, volatility calculation, and statistical analysis to understand market behaviors over a specified period.

## Usage

To use this project, follow the steps below:

1. Download or clone this repository to your local machine.
2. Ensure you have the required datasets available in your project directory. The expected dataset file is `oxfordmanrealizedvolatilityindices.csv`.
3. Run the main script to perform the analysis. The script will:
   - Clean and preprocess the data.
   - Calculate the volatility measures for different symbols.
   - Perform a linear regression analysis to estimate the Hurst exponent and analyze the market's behavior.

### Example

Here's a simple example of how to run a segment of the code:
data = pd.read_csv('oxfordmanrealizedvolatilityindices.csv')

data['Symbol'] = data['Symbol'].str.lstrip('.')
unique_symbols = data['Symbol'].unique()

print(unique_symbols)

## Features

Data Preprocessing: Cleans and prepares the data for analysis.
Volatility Calculation: Utilizes logarithmic returns to calculate volatility measures for different market symbols.
Linear Regression Analysis: Estimates the Hurst exponent for different symbols to analyze market behavior.
Visualization: Generates plots to visually interpret the volatility and regression analysis results.