# E-Commerce Sales Analysis

Analysis of two years of online store data (2024-2025) to understand revenue, profit, customer value and returns, with an interactive dashboard.

![Dashboard preview](dashboard_preview.png)

**Live dashboard:** https://bharath-0917.github.io/E-Commerce-sales-analysis/dashboard/

## Business questions
- How are revenue and profit changing over time?
- Which categories, products and states sell the most?
- Which acquisition channels bring the most valuable customers?
- Where are returns hurting the business?

## Data
Four related tables: customers (3,600), products (90), orders and order items (15,608 line items). Period: January 2024 to December 2025.

## Process
1. Checked each table for missing values and duplicates.
2. Removed duplicate orders and standardised category names.
3. Filled missing unit prices using each product's list price.
4. Merged the four tables into one dataset (`Cleaned_E-commerce_data.csv`).
5. Calculated revenue (quantity x price - discount), cost and profit.
6. Analysed completed orders only, then built the dashboard.

## Key findings (completed orders)
- Revenue is $1.88M with $925K profit (49.2% margin). Revenue grew 21% from 2024 to 2025.
- November is the peak month in both years, so the business is seasonal.
- Furniture earns the most revenue ($322.8K, 17.2%) but has the lowest margin (46.2%) and by far the highest return rate (11.8% vs 4.9% overall).
- Storage has the highest margin (55.6%).
- Referral customers spend the most (about $1,105 each). Paid social customers spend about 40% less (about $649).
- California is the top state ($256.4K, 13.6% of revenue).

## Recommendations
1. Investigate why Furniture is returned so often (damage, sizing or quality).
2. Invest more in referral and organic search.
3. Review paid social and affiliate spending.
4. Plan stock and campaigns early for November.

## Assumptions
- Profit does not include shipping fees.
- Return rate = returned items / all items.

## Tools
Python (Pandas, Matplotlib), Google Colab, Power BI for the interactive dashboard.
