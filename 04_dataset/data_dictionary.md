# Data Dictionary — E-commerce Sales Dataset

## 1. Dataset Overview

The dataset contains synthetic e-commerce transaction records used for this simulated analytics project.

| Attribute | Description |
|---|---|
| Original records | 304 rows |
| Original columns | 10 columns |
| Business domain | E-commerce sales |
| Time period analyzed | January–October 2025 |
| Data type | Synthetic practice data |

## 2. Column Definitions

| Column | Data Type | Description |
|---|---|---|
| Order_ID | Text | Identifier assigned to an order |
| Order_Date | Date | Date of the transaction |
| Product | Text | Name of the purchased product |
| Category | Text | Product category |
| Quantity | Numeric | Number of units purchased |
| Unit_Price | Numeric | Price per unit |
| Discount | Numeric | Discount rate applied |
| Region | Text | Sales region |
| Sales_Channel | Text | Channel through which the order was placed |
| Order_Status | Text | Current order status |

## 3. Important Business Fields

**Order_Status**

Used to determine which transactions are eligible for revenue analysis.

Observed statuses include:

- Completed
- Returned
- Cancelled

**Discount**

Represents the discount rate used in the revenue calculation.

The observed values range from 0 to 0.15.

**Quantity and Unit_Price**

Both fields must contain valid positive values for a transaction to be included in revenue analysis.

## 4. Derived Fields

The analysis process uses additional calculated fields.

| Derived Field | Description |
|---|---|
| Revenue | Quantity × Unit Price × (1 - Discount) |
| Invalid_Quantity | Flag for missing or non-positive Quantity |
| Invalid_Unit_Price | Flag for missing or non-positive Unit Price |

## 5. Data Interpretation Notes

- Missing Product, Region, or Sales_Channel values are represented as Unknown for dimension-based analysis.
- Unknown is a reporting label, not an actual product, region, or sales channel.
- Missing or invalid numerical values are not treated as valid revenue inputs.
- Revenue analysis follows the project's Completed-order business rule.

---

**Dataset Classification:** Synthetic data for portfolio practice.