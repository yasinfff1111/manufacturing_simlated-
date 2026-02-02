# Business Simulation Dataset

This repository contains a Business Simulation Dataset designed to simulate a realistic business environment for analyzing product costs, sales history, market conditions, and key performance indicators (KPIs). The dataset is ideal for data analysis, forecasting, and decision-making scenarios in business operations.

## Table of Contents

- [Dataset Overview](#dataset-overview)
- [File Structure](#file-structure)
- [Data Columns](#data-columns)
  - [Products Sheet](#products-sheet)
  - [Costs Sheet](#costs-sheet)
  - [Sales History Sheet](#sales-history-sheet)
  - [Market Data Sheet](#market-data-sheet)
  - [Analysis Sheet](#analysis-sheet)
- [Data Integrity](#data-integrity)
- [Usage](#usage)
- [License](#license)

## Dataset Overview

This dataset simulates a business environment with a focus on product sales, costs, market conditions, and financial analysis. It includes data for 500 unique products, with sales and cost data spanning 18 months of historical data and 6 months of forecasted data.

The dataset is structured into 5 separate sheets in an Excel file, each containing different types of data crucial for analyzing the business.

## File Structure

The Excel file contains the following sheets:

1. Products: Contains information about each product, including its lifecycle stage, price sensitivity, and category.
2. Costs: Includes costs associated with each product, such as fixed and variable costs, logistics costs, marketing costs, and cost trends.
3. Sales_History: Simulates the historical monthly sales data for each product, including the number of units sold, unit price, and promotion effects.
4. Market_Data: Models external market conditions, such as demand, seasonality, competition intensity, and economic factors.
5. Analysis: Contains key performance indicators (KPIs) like gross margin, profit, profit margin, break-even units, forecasted units sold, and risk level.

## Data Columns

### Products Sheet

The Products sheet contains the following columns:

| Column Name            | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| product_id           | Unique identifier for each product                                           |
| product_name         | Name of the product (e.g., Product_001)                                      |
| category             | Product category (e.g., Electronics, Clothing, Furniture)                    |
| brand                | Brand name of the product (e.g., Brand_01)                                  |
| launch_date          | Launch date of the product (Date when the product was launched)             |
| product_lifecycle_stage | Lifecycle stage (e.g., Introduction, Growth, Maturity, Decline)            |
| price_sensitivity    | Price sensitivity of the product (Elastic, Inelastic)                       |
| quality_score        | Quality score of the product (Scale: 1–10)                                  |

### Costs Sheet

The Costs sheet includes the following columns:

| Column Name             | Description                                                                 |
|-------------------------|-----------------------------------------------------------------------------|
| product_id            | Unique identifier for each product (links to Products sheet)                |
| fixed_cost            | Fixed monthly costs associated with the product                             |
| variable_cost_per_unit| Variable cost per unit (cost to produce one unit of the product)            |
| logistics_cost        | Logistics cost per unit                                                     |
| marketing_cost        | Marketing cost per unit                                                     |
| total_unit_cost       | Total cost per unit (sum of variable cost, logistics cost, and marketing cost)|
| cost_trend            | Trend in cost (Increasing, Stable, or Decreasing)                           |

### Sales History Sheet

The Sales_History sheet contains sales data for each product across 18 months, including:

| Column Name             | Description                                                                 |
|-------------------------|-----------------------------------------------------------------------------|
| product_id            | Unique identifier for each product (links to Products sheet)                |
| date                  | Month of the sale                                                           |
| units_sold            | Number of units sold in the month                                           |
| unit_price            | Price at which the product was sold during the month                        |
| revenue               | Total revenue from the product in the month (units_sold * unit_price)       |
| discount_rate         | Discount rate applied to the product (0-1)                                  |
| promotion_flag        | Flag indicating if the product was on promotion (0 for no, 1 for yes)       |

### Market Data Sheet

The Market_Data sheet includes external factors affecting product sales:

| Column Name             | Description                                                                 |
|-------------------------|-----------------------------------------------------------------------------|
| date                  | Month of the market data                                                   |
| product_id            | Unique identifier for each product (links to Products sheet)                |
| market_demand_index   | Demand index (range from 0.5 to 1.5, with 1 as normal demand)              |
| seasonality_index     | Seasonality index (reflects seasonal demand patterns)                       |
| competition_intensity | Competition intensity (Low, Medium, High)                                   |
| economic_index        | Economic conditions index (reflecting overall market conditions)            |
| holiday_flag          | Flag indicating if the month is a major holiday (0 for no, 1 for yes)      |

### Analysis Sheet

The Analysis sheet contains key performance indicators and calculated metrics for each product:

| Column Name             | Description                                                                 |
|-------------------------|-----------------------------------------------------------------------------|
| product_id            | Unique identifier for each product (links to Products sheet)                |
| date                  | Month of the analysis                                                        |
| gross_margin          | Gross margin (revenue - cost of goods sold)                                  |
| profit                | Profit (gross margin - fixed costs)                                          |
| profit_margin         | Profit margin (profit as a percentage of revenue)                           |
| break_even_units      | Break-even units (number of units required to cover fixed costs)            |
| forecast_units_sold   | Forecasted units sold for the future months based on historical trends      |
| risk_level            | Risk level of the product (Low, Medium, High) based on profit margin and volatility |

## Data Integrity

- No contradictions: Ensure consistency in product_id across all sheets.
- Logical relationships: Prices, costs, and quantities should align with real-world business scenarios.
- No missing data: All products should have valid data for each sheet, with at least 500 rows per sheet.
- Quality: The dataset ensures that high-quality products have higher costs and prices.

## Usage
This dataset is designed for use in various data analysis, forecasting, and business decision-making scenarios. It can be used for:
- Financial analysis: Estimating gross margin, profit, and break-even points.
- Sales forecasting: Predicting future sales based on historical data and market conditions.
- Risk analysis: Identifying products with high operational risks based on profit margins and demand volatility.
- Market analysis: Understanding the effect of market factors like seasonality and competition on sales.

## License

This dataset is available for educational, analytical, and research purposes. You are free to use, modify, and share it under the terms of the MIT License.

---

Feel free to copy this README.md file, adjust any specific information as needed, and upload it to your GitHub repository. This version provides a detailed and clear explanation of the dataset's structure, purpose, and usage, formatted appropriately for GitHub.
