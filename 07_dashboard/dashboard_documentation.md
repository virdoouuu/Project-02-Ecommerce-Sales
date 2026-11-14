# Power BI Dashboard Documentation

## 1. Dashboard Overview

The dashboard provides a visual summary of e-commerce sales performance from January to October 2025.

It was developed in Power BI using the validated revenue analysis dataset.

## 2. Dashboard Components

### KPI Cards

| KPI | Value |
|---|---:|
| Total Revenue | £37,207.55 |
| Total Quantity | 648 |
| Total Orders | 185 |
| Average Order Revenue | £201.12 |

### Monthly Revenue Trend

A line chart showing monthly revenue from January to October 2025.

Purpose:
- Identify revenue changes over time.
- Highlight high- and low-performing months.
- Support further investigation of unusual changes.

### Top 10 Products by Revenue

A horizontal bar chart showing the ten highest-revenue products.

Purpose:
- Compare product revenue.
- Identify the leading product.
- Support product performance monitoring.

### Revenue by Region

A horizontal bar chart showing revenue contributions by region.

Purpose:
- Compare regional revenue.
- Identify the strongest revenue-generating region.
- Highlight missing region information under Unknown.

### Revenue by Category

A column chart comparing revenue across product categories.

Purpose:
- Identify the strongest category.
- Understand category-level revenue concentration.

### Revenue by Sales Channel

A column chart comparing revenue across sales channels.

Purpose:
- Identify the leading channel by revenue.
- Compare the contribution of different channels.
- Highlight missing channel information under Unknown.

## 3. KPI Definitions

**Total Revenue**

Sum of Revenue for valid completed orders.

**Total Orders**

Distinct count of Order_ID in the validated revenue dataset.

**Total Quantity**

Sum of Quantity for valid completed orders.

**Average Order Revenue**

Total Revenue divided by Total Orders.

## 4. Revenue Calculation

`Revenue = Quantity × Unit_Price × (1 - Discount)`

Only valid Completed orders are included.

## 5. Dashboard Design Principles

The dashboard was designed to:

- Present important KPIs at the top.
- Use charts that are appropriate for comparisons and trends.
- Keep labels and titles understandable.
- Show missing descriptive information rather than hiding it.
- Make the most important sales findings easy to identify.

## 6. Screenshot

The final dashboard screenshot is stored in:

`dashboard_screenshot.png`

## 7. Limitations

The dashboard reports revenue and sales quantity. It does not represent profit, marketing ROI, or inventory performance.

---

**Tool:** Microsoft Power BI  
**Project:** E-commerce Sales Performance Analysis