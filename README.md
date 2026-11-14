# E-commerce Sales Performance Analysis

**Project Type:** Data Cleaning, Exploratory Data Analysis, Business Intelligence  
**Tools:** Python, Pandas, Google Colab, Power BI  
**Project Status:** Completed — Practice Portfolio Project

> **Portfolio disclaimer:** This is a simulated freelance data analytics project using a synthetic e-commerce dataset. The client scenario and business requirements were created for learning and portfolio development. This was not paid client work.

## 1. Project Overview

This project analyzes e-commerce sales data to help a business understand its sales performance, identify its strongest products and sales channels, and evaluate revenue across regions and product categories.

The work covers data quality assessment, data cleaning, revenue validation, exploratory data analysis, KPI development, and dashboard creation.

The final deliverable is a Power BI dashboard supported by business insights and recommendations.

## 2. Business Questions

The analysis was designed to answer the following questions:

1. How much revenue did the business generate?
2. How many valid completed orders were recorded?
3. How many product units were sold?
4. What was the average revenue per order?
5. Which products generated the highest revenue?
6. Which regions contributed the most revenue?
7. Which product categories performed best?
8. Which sales channels generated the most revenue?
9. How did revenue change from January to October 2025?

## 3. Executive Summary

The analysis identified **£37,207.55 in total revenue** from **185 valid completed orders**, with **648 units sold**.

The 27-inch Monitor was the highest-revenue product, while Electronics was the leading product category. West generated the highest regional revenue, and Social Media was the strongest sales channel by revenue.

Revenue peaked in July 2025, declined in September, and recovered in October.

These findings highlight the products, regions, categories, and channels that deserve further business attention.

## 4. Key Performance Indicators

| KPI | Result |
|---|---:|
| Total Revenue | £37,207.55 |
| Total Orders | 185 |
| Total Quantity Sold | 648 |
| Average Revenue per Order | £201.12 |

**KPI definitions**

- **Total Revenue:** Sum of revenue from valid completed orders.
- **Total Orders:** Number of distinct valid completed orders.
- **Total Quantity:** Total units sold in valid completed orders.
- **Average Revenue per Order:** Total Revenue divided by Total Orders.

## 5. Data Cleaning and Validation

The original dataset contained 304 rows.

The cleaning process identified and handled the following issues:

- 4 exact duplicate rows were removed.
- 300 rows remained after exact duplicate removal.
- Missing values were identified in Order Date, Product, Quantity, Unit Price, Region, and Sales Channel.
- Invalid quantities and unit prices were flagged.
- Product, region, and sales channel values were standardized for analysis.
- Missing category labels were retained and represented as Unknown rather than removing their revenue contributions.

### Revenue calculation

Revenue was calculated using:

`Revenue = Quantity × Unit Price × (1 - Discount)`

Only orders with `Completed` status and valid positive Quantity and Unit Price were included in the revenue analysis.

After validation:

- Completed orders after duplicate removal: 187
- Invalid completed orders excluded from revenue analysis: 2
- Valid revenue orders: 185

Cancelled and Returned orders were excluded according to the project business rules.

## 6. Business Insights and Recommendations

### Insight 1 — Product Performance

The **27-inch Monitor** generated the highest revenue at **£14,705.85**, contributing approximately **39.5% of total revenue**.

**Business recommendation:** Monitor stock availability and product performance for the 27-inch Monitor. Its high revenue contribution makes it an important product to track.

### Insight 2 — Regional Performance

The **West region** generated the highest revenue at **£13,751.56**, approximately **37.0% of total revenue**.

**Business recommendation:** Investigate what may be contributing to West's stronger performance and assess whether effective sales approaches can be adapted for other regions.

### Insight 3 — Category Performance

The **Electronics** category generated **£20,812.88**, approximately **55.9% of total revenue**.

**Business recommendation:** Continue monitoring Electronics performance while evaluating opportunities to improve revenue from other categories.

### Insight 4 — Sales Channel Performance

**Social Media** generated the highest channel revenue at **£15,463.27**, approximately **41.6% of total revenue**.

**Business recommendation:** Review campaign performance and marketing costs before deciding whether to increase Social Media investment. Revenue alone does not establish marketing profitability.

### Insight 5 — Monthly Revenue Trend

Revenue reached its highest monthly value in **July 2025 at £5,341.81**. Revenue remained high in August, declined in September, and recovered in October to **£4,672.85**.

**Business recommendation:** Investigate the factors behind the September decline and October recovery before making operational or marketing decisions.

## 7. Data Quality Considerations

Some transactions had missing descriptive information.

Their revenue contributions were retained and grouped under Unknown:

| Dimension | Revenue |
|---|---:|
| Product | £438.00 |
| Region | £61.16 |
| Sales Channel | £85.46 |

These values should not be interpreted as zero revenue. They represent revenue whose corresponding descriptive field was not recorded.

## 8. Dashboard

The Power BI dashboard contains:

- Total Revenue
- Total Orders
- Total Quantity
- Average Revenue per Order
- Monthly Revenue Trend
- Top 10 Products by Revenue
- Revenue by Region
- Revenue by Category
- Revenue by Sales Channel

Dashboard screenshot: `07_Dashboard/dashboard_screenshot.png`

## 9. Limitations

This analysis focuses on revenue and sales volume. The dataset does not provide enough information to determine:

- Product profitability or gross margin.
- Marketing return on investment.
- Reasons behind monthly revenue changes.
- Causes of regional performance differences.
- Inventory availability or stock-out effects.
- Whether returned orders received full or partial refunds.

The findings describe observed sales patterns and should not be interpreted as proof of causation.

## 10. Tools and Skills Demonstrated

- Python and Pandas for data cleaning and analysis.
- Data quality checks and validation.
- Revenue calculations and KPI development.
- Exploratory Data Analysis (EDA).
- Power BI dashboard development.
- DAX measures.
- Business insight communication and recommendations.

---

**Project classification:** Simulated freelance portfolio project using synthetic data.