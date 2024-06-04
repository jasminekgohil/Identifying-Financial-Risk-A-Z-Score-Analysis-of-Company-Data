# Identifying-Financial-Risk-A-Z-Score-Analysis-of-Company-Data

This project analyzes a dataset of companies to assess their financial health using a Z-score metric. Here's a breakdown of the key steps:

**Data Cleaning and Preprocessing:**
* The project combines various financial data points for each company.
* It addresses outliers in several columns using a method called Winsorization, which caps extreme values to a specific range.
* The natural logarithm is applied to the "total assets" column to reduce skewness (lopsided distribution).

**Z-Score Calculation:**
A Z-score is calculated for each company based on a weighted formula that considers five financial ratios:
* Current ratio (net current assets / total assets)
* Quick ratio (liquid assets / current liabilities)
* Operating margin (earnings before interest and taxes / total assets)
* Debt-to-equity ratio
* Sales to total assets ratio
Higher Z-scores indicate better financial health and lower risk of bankruptcy.

**Analysis of Z-Scores:**
* The analysis finds that, on average, companies in the dataset have a slightly negative Z-score, suggesting potential financial concerns.
* There's a significant spread of Z-scores, with some companies exhibiting strong financial health (high Z-scores) and others facing potential distress (low Z-scores).
* The analysis explores Z-scores across different industry sectors (e.g., energy, healthcare, IT). It reveals interesting trends like:
* Health care sector having a negative average Z-score, possibly due to regulatory pressures and competition.
* Utilities sector having lower Z-scores but with less variation, reflecting their stable but less profitable nature.

**Regression Analysis:**
* A linear regression model is built to explore the relationship between a company's log(sales) and its Z-score.
* The model explains 13.8% of the variation in Z-scores, indicating a statistically significant but not very strong connection between sales and financial health.
* Companies with higher log(sales) tend to have better Z-scores on average.

Overall, this project demonstrates a data-driven approach to assessing company financial health using Z-scores and basic statistical analysis. It also highlights the importance of considering industry-specific factors when interpreting financial metrics.
