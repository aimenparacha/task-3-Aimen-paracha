# DecodeLabs · Project 4 — Data Visualization

**Batch 2026 | Commerce Analytics Dashboard**

-----

##  File Overview

**File Name:** `DecodeLabs_Project4_Dashboard.xlsx`
**Dataset Period:** January 2023 – June 2025
**Total Orders:** 1,200
**Total Revenue:** $1,264,762
**Products Covered:** Chair, Printer, Laptop, Tablet, Monitor, Desk, Phone

-----

##  Sheet Guide

### 1. Summary

The main dashboard sheet. Contains:

- 5 KPI cards: Total Revenue, Total Orders, Avg Order Value, Delivery Rate, Top Channel
- Key Insights panel highlighting critical findings from the data

### 2. By Product

- Table: Product-wise Orders, Total Revenue, and Average Order Value
- Chart: Column bar chart comparing revenue across all 7 products
- **Key Finding:** Chair and Printer lead at ~$195K each. Laptop has the highest average order value at $1,111.

### 3. Monthly Trend

- Table: Month-by-month revenue for all 30 months (Jan 2023 – Jun 2025)
- Chart: Line chart showing revenue fluctuation over time
- **Key Finding:** Peak month was June 2024 at $68,068. Lowest was April 2023 at $27,751. Revenue shows cyclical volatility with no consistent upward trend.

### 4. Order Status

- Table: Breakdown of orders and revenue by status (Cancelled, Returned, Pending, Shipped, Delivered)
- Chart: Doughnut chart showing proportion of each status
- **Key Finding:** 41.4% of orders are either Cancelled (20.8%) or Returned (20.6%). Only 19.3% of orders were successfully Delivered — a major operational red flag.

### 5. Channels

- Table 1: Revenue and Orders by Referral Source (Instagram, Email, Google, Facebook, Referral)
- Table 2: Revenue and Orders by Payment Method (Credit Card, Online, Cash, Gift Card, Debit Card)
- Charts: Horizontal bar charts for both tables
- **Key Finding:** Instagram is the top acquisition channel at $275K. All payment methods are fairly balanced; Credit Card leads at $263K.

### 6. Coupon Usage

- Table: Orders count and percentage share for each coupon code (FREESHIP, WINTER15, SAVE10, No Coupon)
- Chart: Pie chart showing coupon distribution
- **Key Finding:** FREESHIP is the most used coupon (313 orders, 26%). 309 orders (25.8%) used no coupon at all, indicating strong organic demand.

### 7. Sheet1 (Raw Data)

The original dataset — untouched. All 1,200 rows with 14 columns:
`OrderID, Date, CustomerID, Product, Quantity, UnitPrice, ShippingAddress, PaymentMethod, OrderStatus, TrackingNumber, ItemsInCart, CouponCode, ReferralSource, TotalPrice`

-----

##  Key Insights Summary

|#|Insight          |Detail                                                                           |
|-|-----------------|---------------------------------------------------------------------------------|
|1| High Loss Rate |41.4% of orders cancelled or returned. Needs urgent operational review.          |
|2| Top Products   |Chair & Printer top revenue (~$195K each). Laptop has highest avg order ($1,111).|
|3| Best Channel   |Instagram drives the most revenue at $275K across 259 orders.                    |
|4| Payment Balance|All 5 payment methods are evenly split. Credit Card leads marginally at $263K.   |
|5| Coupon Insight |FREESHIP most popular. 26% of customers buy without any coupon.                  |

-----

## ⚙ Technical Notes

- All summary tables use live Excel formulas (`SUM`, `AVERAGE`) — values update if source data in Sheet1 is changed.
- Charts are embedded directly in their respective sheets.
- No formula errors in the file (verified clean).
- Built with: Python (pandas, openpyxl)

-----

*DecodeLabs · Data Analytics Training Kit · Batch 2026*
