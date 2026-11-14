# Project Brief — E-commerce Sales Analysis

## 1. Project Information

| Item | Details |
|---|---|
| Client | Daniel (Simulated Client) |
| Business Type | E-commerce |
| Project Type | Sales Data Cleaning and Analysis |
| Budget | $30 (Simulated) |
| Deadline | 3 days (Simulated) |
| Dataset | Synthetic e-commerce sales dataset |
| Original Dashboard Request | Excel Dashboard |
| Final Dashboard Tool | Power BI |

**Project Disclaimer:** This is a simulated freelance project created for learning and portfolio development. The client scenario, business requirements, and dataset are fictional. No paid client engagement took place.

## 2. Client Background

Daniel is the owner of an e-commerce business who wants to better understand the company's sales performance.

The business has transaction data containing information about orders, products, quantities, prices, discounts, sales regions, sales channels, and order statuses.

However, the client needs the data to be cleaned and analyzed before it can be used to support business decisions.

## 3. Client Request

The client requested assistance with the following tasks:

1. Clean and prepare the sales dataset.
2. Identify the best-performing products based on revenue.
3. Analyze sales performance across different regions.
4. Identify revenue trends over time.
5. Create a dashboard to present the findings clearly.

The original request specified an Excel dashboard.

For this portfolio exercise, the implementation was adapted to Python and Power BI to demonstrate data cleaning, analytical processing, and interactive business reporting.

## 4. Dataset Overview

The project uses a synthetic dataset containing 304 original records and 10 columns.

| Column | Description |
|---|---|
| Order_ID | Unique order identifier |
| Order_Date | Date of the transaction |
| Product | Product name |
| Category | Product category |
| Quantity | Number of units purchased |
| Unit_Price | Price per unit |
| Discount | Discount applied to the order |
| Region | Sales region |
| Sales_Channel | Channel used for the sale |
| Order_Status | Transaction status |

## 5. Project Scope

### In Scope

- Inspect the original dataset.
- Identify duplicate records.
- Identify missing and invalid values.
- Standardize relevant categorical fields.
- Validate revenue calculations.
- Analyze completed and valid transactions.
- Calculate key performance indicators.
- Analyze product, regional, category, channel, and monthly revenue performance.
- Build a Power BI dashboard.
- Prepare business insights and recommendations.

### Out of Scope

The available dataset does not support a complete analysis of:

- Profitability and gross margin.
- Marketing return on investment.
- Inventory availability.
- Customer lifetime value.
- Reasons behind changes in sales performance.

These topics would require additional business data.

## 6. Business Rules and Assumptions

The following rules were applied for this analysis:

1. Only orders with `Completed` status are eligible for revenue analysis.
2. Cancelled and Returned orders are excluded.
3. Orders with missing or non-positive Quantity are excluded from revenue analysis.
4. Orders with missing or non-positive Unit_Price are excluded from revenue analysis.
5. Revenue is calculated using:

   `Revenue = Quantity × Unit_Price × (1 - Discount)`

6. Exact duplicate records are removed during data preparation.
7. Missing descriptive values are retained and represented as `Unknown` in relevant analysis dimensions rather than automatically removing their revenue.

**Important assumption:** Returned orders are fully excluded from the analysis. In a real client engagement, the refund treatment and revenue recognition rules should be confirmed with the client.

## 7. Expected Deliverables

The expected project outputs are:

- Cleaned and validated sales data.
- Data cleaning documentation.
- Exploratory data analysis.
- KPI calculations.
- Power BI dashboard.
- Business insights and recommendations.
- Final project documentation.

## 8. Project Success Criteria

The project will be considered complete when:

- Data quality issues have been identified and documented.
- Revenue calculations have been validated.
- KPIs are consistent with the analysis results.
- Dashboard figures match the validated analysis.
- Business findings are understandable to a non-technical audience.
- Recommendations are supported by the available data.
- Project files and documentation are organized for handover.

---

**Document Type:** Simulated Client Project Brief  
**Project:** E-commerce Sales Performance Analysis