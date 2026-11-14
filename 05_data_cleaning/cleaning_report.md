# Data Cleaning Report

## 1. Objective

The purpose of data cleaning was to assess the quality of the original e-commerce dataset, identify problematic records, and prepare reliable data for sales analysis.

The original dataset was preserved as the reference source. Cleaning and validation were performed on a working copy.

## 2. Initial Data Assessment

| Metric | Result |
|---|---:|
| Original Rows | 304 |
| Exact Duplicate Rows Removed | 4 |
| Rows After Duplicate Removal | 300 |

## 3. Data Quality Findings

The initial assessment identified missing values in the following fields:

| Column | Missing Values |
|---|---:|
| Order_Date | 1 |
| Product | 1 |
| Quantity | 1 |
| Unit_Price | 1 |
| Region | 1 |
| Sales_Channel | 1 |

Discount and Category did not contain missing values in the initial assessment.

Additional quality issues included:

- One zero Quantity value.
- One negative Unit_Price value (-12.5).
- Mixed date formats.
- Duplicate records.

## 4. Cleaning Actions

| Issue | Action |
|---|---|
| Exact duplicate rows | Removed from the working dataset |
| Mixed date formats | Standardized and parsed into a consistent date format |
| Missing descriptive fields | Preserved and represented as Unknown in relevant reporting dimensions |
| Zero or missing Quantity | Flagged as invalid for revenue analysis |
| Negative or missing Unit_Price | Flagged as invalid for revenue analysis |
| Discount | Validated against the expected 0–1 range |

The original data was not silently overwritten. Problematic records were retained in the cleaned working dataset where appropriate and flagged for auditability.

## 5. Revenue Validation

Revenue was calculated using:

`Revenue = Quantity × Unit_Price × (1 - Discount)`

Only Completed orders with valid positive Quantity and Unit_Price were included.

| Validation Metric | Result |
|---|---:|
| Completed Orders After Deduplication | 187 |
| Invalid Completed Orders Excluded | 2 |
| Valid Revenue Orders | 185 |
| Total Revenue | £37,207.55 |

## 6. Data Quality Flags

| Validation | Result |
|---|---:|
| Invalid Quantity Flags | 2 |
| Invalid Unit Price Flags | 2 |
| Minimum Discount | 0.00 |
| Maximum Discount | 0.15 |
| Discount Outside 0–1 | 0 |

**Important:** The invalid Quantity and Unit Price flag totals include missing values and non-positive values. They should not be added together as if they represented four separate records.

## 7. Final Analysis Dataset

The final revenue analysis dataset contains:

- 185 valid completed orders.
- £37,207.55 total revenue.
- 648 total units sold.

## 8. Conclusion

The cleaning process removed four exact duplicate records and identified missing and invalid values.

The resulting analysis dataset was restricted to valid Completed transactions and validated against the revenue calculation rules.

Descriptive missing values were retained as Unknown in reporting dimensions to preserve valid revenue contributions.

---

**Report Type:** Data Cleaning and Validation  
**Project:** E-commerce Sales Performance Analysis