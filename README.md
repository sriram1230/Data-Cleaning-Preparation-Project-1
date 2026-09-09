# Project 1 – Data Cleaning & Preparation
## Overview
This project was completed as part of the DecodeLabs Industrial Training Kit – Data Analytics track.
The objective was to clean and validate a raw dataset by identifying missing values, checking duplicate IDs, verifying data formats, and validating numerical consistency before further analysis.

## Dataset Summary
- **Records:** 1,200
- **Columns:** 14
- **Primary identifier checked:** `OrderID`
- **Date range:** 2023-01-01 to 2025-06-30

## Cleaning & Validation Performed
### 1. Duplicate ID Check
- Checked `OrderID` for duplicate values.
- **Result:** 0 duplicate OrderIDs found.

### 2. Missing Values
- Checked the dataset for missing values.
- `CouponCode` contains **309 blank values**.
- These blanks were retained because a blank coupon code can represent an order where no coupon was recorded/applied.
- `Date` contains **0 blank values**.

### 3. Date Format Verification
- Verified the `Date` column.
- Dates are consistently represented in **YYYY-MM-DD** format.
- **Missing dates:** 0

### 4. Numeric Data Validation
- `Quantity`: checked for blank, zero, and negative values.
- `UnitPrice`: checked for blank, zero, and negative values.
- `TotalPrice`: checked for blank, zero, and negative values.

Results:
- Invalid Quantity values: **0**
- Invalid UnitPrice values: **0**
- Invalid TotalPrice values: **0**

### 5. Total Price Consistency
Verified:

`TotalPrice = Quantity × UnitPrice`
- **Mismatches found:** 0
## Final Results
| Check | Result |
|---|---:|
| Total records | 1,200 |
| Duplicate OrderIDs | 0 |
| Missing Date values | 0 |
| Blank CouponCode values | 309 |
| Invalid Quantity values | 0 |
| Invalid UnitPrice values | 0 |
| Invalid TotalPrice values | 0 |
| TotalPrice calculation mismatches | 0 |
| Date format | YYYY-MM-DD |

## Tools Used
- Google Sheets
- Microsoft Excel
- Spreadsheet filters and formulas
- Data cleaning and validation techniques

## Learning Outcomes
- Identifying missing data
- Detecting duplicate records
- Verifying date formats
- Validating numerical fields
- Checking calculation consistency
- Preparing reliable data for future analysis

## Conclusion
The dataset was systematically checked for the main data-quality issues required by Project 1. The final validation confirmed **zero duplicate OrderIDs**, **zero missing Date values**, and **no TotalPrice calculation mismatches**. The identified blank `CouponCode` values were retained rather than replaced with fabricated information.

**Project:** DecodeLabs Industrial Training Kit – Data Analytics  
**Milestone:** Project 1 – Data Cleaning & Preparation
