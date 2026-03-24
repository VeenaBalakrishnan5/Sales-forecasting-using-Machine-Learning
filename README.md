# Sales Forecasting using Machine Learning

[cite_start]This project involves the development of a sales forecasting system designed to estimate future revenue and optimize business operations[cite: 1, 2]. [cite_start]By analyzing historical transaction data, the project provides insights into future demand, helping businesses balance inventory levels and allocate resources more efficiently[cite: 2, 3].

## Project Overview
[cite_start]The primary goal of this research is to apply quantitative forecasting methods—using historical data and statistical models—to predict future sales trends[cite: 1, 11]. [cite_start]Accurate forecasts are essential for planning production, managing budgets, and optimizing supply chains[cite: 2, 3].

## Dataset Profile
The analysis is performed on a retail dataset (`stores_sales_forecasting.csv`) containing 2,121 records with 21 distinct features. 
* **Timeframe**: The data spans from January 2014 to December 2017.
* **Categories**: The focus is on the **Furniture** category, including sub-categories like Bookcases, Chairs, Tables, and Furnishings.
* **Key Metrics**: Sales values range from 1.89 to 4,416.17, while profit margins range from -1,862.31 to 1,013.13.

## Key Features & Workflow
* **Data Preprocessing**: 
    * Conversion of 'Order Date' into a standardized datetime format for time-series analysis.
    * Rounding of financial metrics ('Sales' and 'Profit') for consistency.
    * Text normalization (lowercasing and stripping whitespace) to address inconsistent capitalization in columns such as 'City' and 'Product Name'.
* **Feature Engineering**: Removal of redundant identifiers like 'Row ID', 'Order ID', and 'Customer ID' to streamline the analysis.
* **Statistical Analysis**: Identification of high-value outliers in the sales column where the mean significantly exceeds the median.
* **EDA**: Exploratory Data Analysis to identify seasonal trends and geographic factors influencing demand.

## Methodologies
The project explores two main types of sales forecasting:
* [cite_start]**Qualitative**: Subjective methods such as the Delphi method or market research, useful when historical data is limited[cite: 9, 10].
* [cite_start]**Quantitative**: Objective methods using historical numerical data and statistical models to predict future performance[cite: 11].

## Technical Stack
* **Language**: Python
* **Libraries**: `pandas`, `numpy`, `matplotlib`, and `seaborn`
* **Environment**: Jupyter Notebook

## Installation & Setup
To run the analysis:
1.  Install the required dependencies:
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```
2.  Ensure the dataset `stores_sales_forecasting.csv` is in the project directory.
3.  Execute the cells in `sales_forecasting_using_machine_learning.ipynb` to view the data cleaning and EDA steps.
