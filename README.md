# Customer Shopping Behavior Analysis

## Overview

This project analyzes customer shopping behavior using transaction data to identify meaningful patterns and turn them into actionable business insights.

The project follows an end-to-end data analytics workflow, from raw transaction data and exploratory analysis to data cleaning, SQL analysis, Power BI visualization, reporting, and presentation.

## Dataset

The dataset contains **3,900 purchases** and **18 columns** covering customer demographics, purchase details, product preferences, and shopping behavior.

The analysis includes:

- Customer demographics
- Purchase behavior
- Product preferences
- Review ratings
- Shipping choices
- Discount usage
- Subscription status

There are **37 missing review ratings**, which were handled using category-level median imputation.

## Tools & Technologies

- **Python** – Data loading, EDA, data cleaning, and feature engineering
- **Pandas** – Data manipulation and analysis
- **PostgreSQL** – Database storage and SQL analysis
- **SQL** – Business-focused data analysis
- **Power BI** – Interactive dashboard and visualization
- **Excel/CSV** – Data handling and inspection
- **Gamma** – Project presentation
- **Jupyter Notebook** – Python-based analysis

## Project Workflow

### 1. Load & Profile

The raw transaction dataset was loaded into Python and explored using Pandas.

The initial analysis focused on understanding:

- Dataset structure
- Data types
- Summary statistics
- Missing values
- Customer and purchase patterns

### 2. Data Cleaning

The dataset was cleaned and prepared for further analysis.

Key steps included:

- Inspecting the dataset using `df.info()` and `df.describe()`
- Handling missing Review Rating values using the median of each product category
- Standardizing column names to `snake_case`
- Checking redundant fields
- Preparing the cleaned dataset for PostgreSQL

### 3. Feature Engineering

New features were created to support customer behavior analysis:

- `age_group`
- `purchase_frequency_days`

The `promo_code_used` field was also checked against `discount_applied` for redundancy.

### 4. PostgreSQL & SQL Analysis

The cleaned DataFrame was loaded into PostgreSQL for SQL-based analysis.

Ten business-focused SQL questions were analyzed across areas such as:

- Revenue by gender
- Revenue by age group
- Subscription behavior
- Top-rated products
- Top products by category
- Discount dependence
- Shipping behavior
- Customer segments
- Repeat buyers
- Loyalty opportunities

### 5. Power BI Dashboard

The analysis was converted into an interactive Power BI dashboard.

The dashboard includes views for:

- Subscription status
- Category revenue
- Category sales
- Shipping type
- Gender distribution
- Age distribution

Key dashboard metrics include:

- **3.9K customers**
- **$59.76 average purchase amount**
- **3.75 average review rating**

### 6. Report & Presentation

The final analysis was documented in a project report and presented through a PowerPoint presentation created using Gamma.

The presentation summarizes the analytical workflow, key findings, business opportunities, and recommendations.

## Dashboard

The Power BI dashboard provides a decision-oriented view of customer shopping behavior.

It allows the analysis to move from overall KPIs to specific questions around customers, categories, age groups, gender, subscription status, and purchasing behavior.

## Key Results

The analysis identified several important patterns:

- **Male customers generated higher revenue** than female customers in the analyzed dataset.
- **Young Adults** were the highest-revenue age group, generating **$62,143** in revenue.
- Customers using discounts spent above the average purchase amount, with **839 customers** identified in this analysis.
- **Gloves, Sandals, Boots, Hat, and Skirt** were among the highest-rated products.
- **Jewelry, Blouse, Sandals, and Jacket** ranked strongly within their categories by total orders.
- Average purchase amount was **$58.46 for Standard shipping** and **$60.48 for Express shipping**.
- The dataset contained **3,116 loyal customers**, highlighting customer loyalty as a major opportunity.
- There were **1,053 subscribers** compared with **2,847 non-subscribers**.
- The analysis identified opportunities to improve customer loyalty, understand discount dependence, and strengthen subscription and retention strategies.

## How to Run

### Python Analysis

1. Clone or download this repository.
2. Open the Jupyter Notebook.
3. Make sure Python and Pandas are installed.
4. Place the dataset in the required location.
5. Run the notebook cells from top to bottom.

Example:

```bash
pip install pandas jupyter

```bash
pip install pandas jupyter
