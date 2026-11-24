# Retail Sales Exploratory Data Analysis

An end-to-end exploratory data analysis (EDA) project on retail transaction data, built in Google Colab using Python (`pandas` and `matplotlib`) to uncover spending patterns across product categories, customer demographics, and time.

## Project Overview
Retail businesses rely on transaction data to see which products drive revenue, how different customer segments behave, and how sales shift over time. In this project, raw tab-separated retail transaction records were loaded, checked for data quality, segmented across multiple dimensions, and visualized using bar and line charts.

## Workflow & Analysis Steps
- **Data Loading & Cleaning:** Loaded the tab-separated transaction dataset into a `pandas` DataFrame and inspected column types and structure.
- **Data Validation:** Verified that there are no missing values and checked calculation consistency (`Quantity * Price per Unit` vs. `Total Amount`) across records.
- **Category Performance:** Aggregated revenue across product categories (`Electronics`, `Clothing`, and `Beauty`) to identify top-performing lines.
- **Gender Breakdown:** Compared order counts, average order value, and total revenue across Female and Male customers.
- **Age & Category Segmentation:** Grouped customers into age brackets (`18–25`, `26–35`, `36–50`, `51+`) and cross-tabulated spending by product category.
- **Monthly Sales Trend:** Parsed transaction dates into monthly periods to track revenue movement over time.

## Key Findings
- **Top Revenue Category:** Electronics leads overall sales (`156,905`), closely followed by Clothing (`155,580`) and Beauty (`143,515`).
- **Consistent Average Spend by Gender:** Average order value is nearly identical between Female (`456.55`) and Male (`455.43`) buyers, meaning total revenue differences are driven primarily by order volume (`510` vs. `490` orders).
- **Demographic Shifts by Category:** Customers aged `51+` generate the highest spending in Electronics (`55,305`) and Clothing (`46,120`), while the `18–25` age bracket leans slightly more toward Beauty (`31,280`).
- **Broad Mid-Age Engagement:** The `36–50` segment shows strong, balanced activity across all three product categories.

## Repository Contents
- `retail_sales_analysis.ipynb` — Google Colab notebook containing the full data validation, aggregations, summary metrics, and charts.
- Retail transaction dataset file — Tab-separated input data used for the analysis.
- `README.md` — Project documentation and summary of key insights.
