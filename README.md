# Global-Superstore-Analysis
### Project Overview

This project presents an in-depth analysis of the Global Superstore dataset, aimed at deriving actionable business insights from sales, profit, and customer behavior data.
Through exploratory data analysis (EDA), customer segmentation, and time series forecasting, the project identifies revenue drivers, inefficiencies, and opportunities for profit optimization.

The analysis simulates a real-world business analytics workflow, integrating both descriptive and predictive techniques to support data-driven decision-making.

### Objectives

Understand sales and profitability patterns across regions, categories, and sub-categories

Identify high-value and at-risk customers using RFM analysis

Evaluate the impact of discounts and shipping efficiency on profit

Forecast future sales trends using ARIMA time series modeling

Provide strategic recommendations to improve profitability and customer retention

### Dataset Description

Dataset: Global Superstore (Kaggle)

| Column                  | Description                             |
| ----------------------- | --------------------------------------- |
| Order ID                | Unique identifier for each order        |
| Order Date, Ship Date   | Date attributes for time-based analysis |
| Region, Country         | Geographical information                |
| Category, Sub-Category  | Product classification                  |
| Sales, Profit, Discount | Key financial metrics                   |
| Quantity, Shipping Cost | Operational metrics                     |
| Customer ID, Segment    | Customer-level information              |

### Analysis Workflow
1. Data Preparation
    - Dropped irrelevant columns (e.g., Row ID, Postal Code)

    - Created new derived metrics:

        - Profit Margin

        - Sales per Order

        - Shipping Efficiency

2. Exploratory Data Analysis (EDA)

    - KPIs: Total Sales, Total Profit, and Shipping Cost

    - Regional Insights: Central region led both sales and profit performance

    - Category Analysis: Office Supplies had moderate sales but high profitability

    - Sub-category Performance: Identified top 10 sub-categories by both sales and profit

    - Discount vs. Profit: Found that higher discounts do not necessarily increase profit

3. Correlation & Visualization

    - Visualized relationships between numeric variables via a correlation heatmap

    - Observed:

        - Positive correlation among Sales–Quantity–Profit

        - Negative correlation between Profit–Discount and Sales per Order–Shipping Efficiency

4. Customer Segmentation (RFM Analysis)

    - Segmented customers into:

        - Champions

        - Loyal

        - At-Risk

        - Win-Back

    - Highlighted behavioral patterns useful for targeted marketing strategies

5. Pareto (80/20) Analysis

    - Confirmed that a small subset of customers/products contributes to the majority of sales

    - Suggested prioritizing high-performing segments for strategic focus

6. Time Series Forecasting

    - Decomposed monthly sales data into trend, seasonality, and residuals

    - Applied Augmented Dickey-Fuller (ADF) test — revealed non-stationarity

    - Used first-order differencing to achieve stationarity

    - Determined ARIMA(2,1,0) model parameters via ACF and PACF

    - Forecasted upcoming sales trends to support business planning

### Key Insights

    - Sales vs Profit: The South region, despite high sales, lagged in profitability due to discount and shipping costs.

    - Category Optimization: Technology products yielded higher margins than Furniture or Office Supplies.

    - Discount Strategy: Excessive discounting led to profit erosion.

    - Customer Retention: A focused strategy for at-risk and win-back segments can improve recurring revenue.

    - Forecasting Outcome: Expected moderate sales growth trend over the next forecast horizon.
    
### Future Improvements

- Implement an interactive dashboard (e.g., Power BI / Plotly Dash) for dynamic insights

- Explore predictive modeling for customer churn or profit prediction

- Automate RFM segmentation pipeline for real-time reporting

### Business Recommendations

- Optimize discount policies by analyzing elasticity of demand per category

- Focus marketing on “Champion” customers and reactivation campaigns for “At-Risk” groups

- Streamline shipping operations to reduce cost-to-serve in low-profit regions

- Invest in technology category for sustained high-margin growth






