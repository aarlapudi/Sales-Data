## Data Cleaning and Standardization Project
📌 Project Overview

This project focuses on cleaning and standardizing a customer order dataset to prepare it for further analytics and reporting.
The work was carried out using a combination of Python (Pandas) for automation and Excel for manual validation and corrections.

🛠️ Tools & Technologies Used

Python 3.x

Pandas (for data cleaning and transformation)

Jupyter Notebook (for automation)

Microsoft Excel (for manual review, corrections, and validation)

Git & GitHub (for version control and collaboration)

📊 Data Cleaning & Transformation Steps
🔧 Python-Based Cleaning
1️ Phone Number Normalization

Removed unwanted characters (spaces, dashes, parentheses) using str.replace().

Standardized phone numbers by:

Trimming or padding numbers to match country-specific lengths

Adding country codes based on COUNTRY column

Converting to international format: +<CountryCode><Number>

Converted phone numbers to string type to avoid Excel’s automatic number formatting (scientific notation).

2️ Postal Code Fixes

Identified and filled missing postal codes for cities like San Francisco and Los Angeles using a mapping dictionary.

Ensured all postal codes were stored as strings to preserve leading zeros.

 Excel-Based Cleaning

For all other columns, manual review and cleaning were done directly in Excel:

STATE Column → Filled 2500 missing values using city-to-state mapping.

CITY, STATE, COUNTRY → Standardized naming (title case) and removed trailing/leading spaces.

PRODUCT-RELATED COLUMNS (PRODUCTLINE, PRODUCTCODE, MSRP) → Checked for inconsistencies and corrected them.

ORDERDATE Column → Verified date format consistency.

Duplicate Rows → Identified and removed duplicates where necessary.

Other Null Values → Filled missing values appropriately or left them blank if no reliable source existed.

✅ Final Verification

Validated results using Excel filters, pivot tables, and summary checks.

Exported cleaned dataset as updated_dataset.xlsx to preserve formatting.
