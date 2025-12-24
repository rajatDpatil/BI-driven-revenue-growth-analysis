# Customer Shopping Behavior Analysis

## Brief Summary

End-to-end business intelligence project analyzing 3,900+ customer transactions to optimize revenue streams and deliver actionable insights for strategic growth.

## Overview

This project provides a comprehensive analysis of customer shopping behavior to uncover spending patterns, customer segments, and subscription trends. By leveraging data analytics across multiple platforms, the project transforms raw transactional data into strategic business recommendations for revenue maximization and customer retention.

## Problem Statement

Businesses struggle to understand customer purchasing behavior and optimize revenue streams effectively. Key challenges include:
- Identifying high-value customer segments
- Understanding the impact of discounts on profitability
- Determining factors that drive subscription conversions
- Optimizing product positioning and marketing strategies

This project addresses these challenges by analyzing comprehensive transactional data to provide data-driven insights for strategic decision-making.

## Dataset

- **Total Records:** 3,900 customer transactions
- **Features:** 18 columns covering:
  - **Demographics:** Age, Gender, Location, Subscription Status
  - **Purchase Details:** Item Purchased, Category, Purchase Amount, Season, Size, Color
  - **Behavior Metrics:** Discount Applied, Previous Purchases, Frequency, Review Rating, Shipping Type
- **Data Quality:** 37 missing values in Review Rating (handled via median imputation by category)

## Tools and Technologies

- **Python (Jupyter Notebook)** - Data cleaning, EDA, and feature engineering
- **PostgreSQL** - Business analytics and structured querying
- **Power BI** - Interactive dashboard and data visualization
- **Key Libraries:** pandas, numpy, psycopg2

## Methods

### 1. Data Preprocessing (Python)
- Loaded and explored dataset using pandas
- Handled missing values with category-based median imputation
- Engineered features: `age_group`, `purchase_frequency_days`
- Standardized column names to snake_case
- Removed redundant columns after consistency checks
- Connected to PostgreSQL for further analysis

### 2. Business Analysis (SQL)
Executed 10 strategic queries:
- Revenue analysis by gender and age groups
- High-spending discount user identification
- Product performance and rating analysis
- Shipping preference impact on spending
- Subscription vs. non-subscription behavior comparison
- Customer segmentation (New, Returning, Loyal)
- Discount dependency by product
- Repeat buyer subscription correlation

### 3. Visualization (Power BI)
- Built interactive dashboard with revenue breakdowns
- Visualized customer segmentation and behavior trends
- Created product performance metrics
- Displayed subscription impact analysis

## Key Insights

- **Customer Segmentation:** Identified distinct New, Returning, and Loyal customer groups with varying spending patterns
- **Subscription Value:** Subscribers show higher average spend and lifetime value
- **Discount Effectiveness:** Certain customers maintain high spending despite discount usage
- **Age Demographics:** Specific age groups contribute disproportionately to total revenue
- **Repeat Purchase Correlation:** Customers with 5+ purchases show higher subscription likelihood
- **Product Performance:** Top-rated products align with best-selling items, indicating quality-driven purchases

## Dashboard/Model/Output

The Power BI dashboard includes:
- **Revenue Overview:** Total revenue by gender, age group, and subscription status
- **Customer Segmentation View:** Distribution across New, Returning, and Loyal segments
- **Product Analytics:** Top products by category, rating, and discount dependency
- **Behavioral Insights:** Purchase frequency, shipping preferences, and discount impact
- **Interactive Filters:** Dynamic filtering by demographics, product categories, and time periods

## How to Run this Project?

### Prerequisites
- Python 3.8+
- PostgreSQL 12+
- Power BI Desktop
- Required libraries: `pandas`, `numpy`, `psycopg2`

### Steps
1. **Clone the repository**
   ```bash
   git clone <gh repo clone rajatDpatil/BI-driven-revenue-growth-analysis>
   cd customer-shopping-analysis
   ```

2. **Install dependencies**
   ```bash
   pip install pandas numpy psycopg2-binary
   ```

3. **Run data preprocessing**
   - Open `notebooks/customer_analysis_eda.ipynb`
   - Execute all cells to clean and prepare data

4. **Set up PostgreSQL**
   - Create database and update connection credentials
   - Run the notebook to load cleaned data into PostgreSQL

5. **Execute SQL queries**
   - Open `sql/business_queries.sql`
   - Run queries in PostgreSQL to generate insights

6. **View dashboard**
   - Open `dashboard/shopping_behavior_dashboard.pbix` in Power BI Desktop

## Results & Conclusion

The analysis successfully identified key revenue drivers and customer behavior patterns:
- **Revenue Optimization:** Pinpointed high-value customer segments and products
- **Strategic Insights:** Provided actionable recommendations for subscription growth and customer retention
- **Data-Driven Decisions:** Enabled targeted marketing strategies based on demographic and behavioral analysis
- **Profitability Balance:** Highlighted need for discount policy review to maintain margins while boosting sales

**Conclusion:** This project demonstrates how integrated analytics across Python, SQL, and Power BI can transform raw data into strategic business intelligence, driving revenue growth and customer loyalty.

## Future Work

- Implement predictive modeling for customer churn and lifetime value
- Develop recommendation system based on purchase history
- Incorporate real-time analytics for dynamic pricing strategies
- Expand analysis to include seasonal trends and geographic patterns
- Build automated reporting pipeline for continuous monitoring
- Apply machine learning for customer segmentation optimization

## Project Structure

```
customer-shopping-analysis/
│
├── data/
│   ├── raw_data.csv
│   └── cleaned_data.csv
│
├── notebooks/
│   └── customer_analysis_eda.ipynb
│
├── sql/
│   └── business_queries.sql
│
├── dashboard/
│   └── shopping_behavior_dashboard.pbix
│
├── README.md
└── requirements.txt
```

---

**Author:** [Rajat D Patil]  
**Email:** [batm34993@gmail.com]  
**Contact:** [https://www.linkedin.com/in/rajat-d-patil/]
