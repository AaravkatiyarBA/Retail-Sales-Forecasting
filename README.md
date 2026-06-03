# Retail Sales Forecasting & Store Performance Analytics

## Overview

Accurate sales forecasting is essential for retailers to optimize inventory levels, improve workforce planning, manage promotional campaigns, and maximize profitability.

This project combines retail sales analysis, SQL-based business reporting, machine learning forecasting, and Power BI dashboarding to analyze historical sales performance and predict future weekly sales across multiple stores and departments.

The project leverages store-level, department-level, promotional, seasonal, economic, and operational variables to improve forecasting accuracy and generate actionable business insights.

---

## Business Problem

Retail organizations often face challenges such as:

* Inventory stockouts
* Excess inventory holding costs
* Inefficient workforce allocation
* Poor promotional planning
* Revenue volatility

The objective of this project is to analyze historical sales performance and forecast future weekly sales to support better operational and strategic decision-making.

---

## Project Objectives

* Analyze sales performance across stores and departments
* Evaluate the impact of holidays and seasonal trends
* Identify top-performing stores and departments
* Build a machine learning model for weekly sales forecasting
* Generate actionable recommendations for inventory and resource planning

---

## Dataset

The project combines multiple retail datasets including:

### Sales Data

* Weekly Sales
* Store ID
* Department ID
* Date

### Store Data

* Store Type
* Store Size
* Region

### External Factors

* Temperature
* Fuel Price
* CPI
* Unemployment Rate
* Holiday Events
* Markdown Promotions

### Final Dataset

| Metric      | Value    |
| ----------- | -------- |
| Records     | 156,000  |
| Features    | 18+      |
| Stores      | Multiple |
| Departments | Multiple |

---

## Data Engineering

The project involved:

* Data import and cleaning
* SQL-based joins and merges
* Missing value treatment
* Date feature extraction
* Feature engineering
* Dataset consolidation

### Engineered Features

* Month
* Quarter
* Week
* Lag Sales (Previous Week)
* Rolling 4-Week Average

These features helped capture sales momentum and seasonality patterns.

---

## Exploratory Analysis

### Business Questions Addressed

#### Top Performing Stores

Identified stores contributing the highest revenue and sales volume.

#### Department Performance

Compared departmental sales contribution and performance trends.

#### Holiday Impact Analysis

Evaluated how holiday events influenced weekly sales.

#### Seasonal Performance

Analyzed sales behavior across different seasons and promotional periods.

---

## Forecasting Methodology

### Machine Learning Model

The project uses:

**XGBoost Regressor**

### Features Used

* Department
* Store Size
* Store Type
* Region
* Temperature
* Fuel Price
* CPI
* Unemployment
* Holiday Events
* Seasonal Variables
* Promotional Markdowns
* Lag Features
* Rolling Averages

---

## Model Performance

| Metric   | Result |
| -------- | ------ |
| MAE      | 24,905 |
| R² Score | 0.481  |

### Interpretation

* Average forecasting error was approximately 24,905 sales units.
* The model explained approximately 48% of sales variability.
* Lag features and rolling averages significantly improved forecasting capability.

---

## Key Findings

### Holiday Impact

Sales volumes increased during major holiday periods due to promotional activity and increased customer spending.

### Seasonal Trends

Sales patterns varied significantly across seasons, highlighting the importance of seasonal inventory planning.

### Promotional Influence

Markdown campaigns demonstrated measurable effects on sales performance.

### Store Performance

Large-format stores consistently generated higher weekly sales than smaller locations.

---

## Business Recommendations

### 1. Improve Inventory Planning

Use demand forecasts to optimize stock allocation and reduce stockouts.

### 2. Strengthen Holiday Planning

Increase inventory and staffing levels before major holiday periods.

### 3. Target Promotional Investments

Focus markdown budgets on departments and stores with the highest responsiveness.

### 4. Store-Specific Forecasting

Implement localized forecasting models for individual stores and departments.

### 5. Expand Feature Set

Future models can incorporate competitor pricing, regional demographics, and economic indicators.

---

## SQL Analysis Performed

The project includes SQL-based analysis for:

* Departmental Performance Analysis
* Holiday Impact Analysis
* Seasonal Performance Analysis
* Top Stores by Sales
* Dataset Integration and Merging

---

## Technologies Used

### Data Analysis

* Python
* Pandas
* NumPy

### Machine Learning

* XGBoost
* Scikit-Learn

### Visualization

* Power BI

### Database

* SQL

---

## Repository Structure

```text
retail-sales-forecasting/
│
├── data/
│   ├── sales.csv
│   ├── stores.csv
│   ├── features.csv
│   └── retail_master.csv
│
├── notebooks/
│   └── Sales_forecasting.ipynb
│
├── sql/
│   ├── create_import_merge.sql
│   ├── departmental_performance.sql
│   ├── holiday_impact.sql
│   ├── seasonal_performance.sql
│   └── top_stores_sales.sql
│
├── dashboard/
│   └── Retail_Sales_Dashboard.pbix
│
├── output/
│   └── forecast_output.csv
│
└── README.md
```

---

## Future Enhancements

* Store-level forecasting models
* Department-level forecasting models
* Time-series forecasting (Prophet / ARIMA)
* Hyperparameter optimization
* Forecasting dashboard deployment

---

## Author

**Aarav Katiyar**

MBA Candidate | Business Analytics | Forecasting & Market Research

LinkedIn: https://www.linkedin.com/in/aarav-katiyar-65b7b2237/

GitHub: https://github.com/AaravkatiyarBA
