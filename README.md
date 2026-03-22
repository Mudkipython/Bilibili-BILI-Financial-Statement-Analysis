# Bilibili (BILI) Financial Statement Analysis

This directory contains a comprehensive financial statement analysis of **Bilibili Inc. (BILI)**, developed as part of ACCT 626. 

The core of this analysis is the Jupyter Notebook `BILI.ipynb`, which automatically retrieves, processes, and visualizes Bilibili's financial data to extract key insights regarding the company's profitability, liquidity, solvency, efficiency, and growth.

## Project Objectives

1. **Data Retrieval**: Automatically fetch annual and quarterly financial statements using the `yfinance` library.
2. **TTM Construction**: Construct trailing twelve months (TTM) financial data from quarterly figures to provide a smoothed, up-to-date view of the company's performance.
3. **Data Standardization**: Standardize key accounting line items across different financial statements.
4. **Ratio Analysis**: Calculate and evaluate selected financial ratios across multiple dimensions:
   - Profitability
   - Liquidity
   - Solvency
   - Efficiency
   - Growth
   - Cash Flow Quality
5. **Visualization**: Generate clear charts to visualize key financial trends and drivers over time.
6. **Data Export**: Export pristine, structured tables of financial data and ratios for use in formal reporting.

## Key Files

* **`BILI.ipynb`**: The main Jupyter Notebook containing all the Python code for data extraction, manipulation, analysis, and visualization.
* **`bili_output/`**: An automatically generated folder that houses the outputs from the notebook:
  * **`BILI_Financial_Analysis_Notebook_Output_Thousands.xlsx`**: An Excel spreadsheet containing the detailed financial data and calculated ratios. *Note: All amount-based output tables are displayed in thousands.*
  * **Visualizations**:
    * `BILI_revenue_net_income.png`: Trends in total revenue vs. net income.
    * `BILI_margin_trend.png`: Evolution of profit margins over time.
    * `BILI_cash_flow_trend.png`: Operating, investing, and financing cash flow trends.
    * `BILI_liquidity_leverage.png`: Key liquidity and leverage metrics.
    * `BILI_dupont_framework_TTM.png` & `BILI_dupont_drivers.png`: Visual breakdowns of the DuPont analysis framework to pinpoint drivers of Return on Equity (ROE).

## Important Accounting Notes

* **Foreign Private Issuer**: Bilibili is a foreign private issuer. Therefore, its primary annual filing with the SEC is **Form 20-F**, not Form 10-K. This is an important distinction for formal financial reporting and analysis.
* **Unit Convention**: Unless otherwise specified (e.g., in ratio tables where values are unscaled), all financial statement values and amount-based output tables are presented **in thousands**.

## Requirements and Usage

To run the notebook, you will need a Python environment with the following packages installed:
* `pandas`
* `numpy`
* `matplotlib`
* `yfinance`
* `openpyxl` (for Excel export)

You can install these dependencies using pip:
```bash
pip install yfinance openpyxl matplotlib pandas numpy
```

Simply open `BILI.ipynb` in Jupyter Notebook or JupyterLab and run the cells sequentially to reproduce the analysis and generate the output files in the `bili_output` directory.
