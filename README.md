# Customer Call List Data Cleaning Project

This project demonstrates a comprehensive data cleaning workflow using **Pandas** in **Jupyter Notebook** on an Excel dataset: `Customer Call List.xlsx`.

The goal was to clean, standardize, and prepare the dataset for downstream use such as customer outreach, analytics, or modeling.

---

## Files Included

- `Customer Call List.xlsx` – Original raw dataset (Excel format)
- `DataCleaning.ipynb` – Jupyter Notebook with full cleaning steps
- `cleaned_data.xlsx` – Final cleaned dataset (xlsx format)
- `uncleaned_data.xlsx` – Records with null values
---

## Tools & Libraries Used

- **Python**
- **Pandas** – For data manipulation and cleaning
- **Jupyter Notebook** – Interactive development environment

---

## Cleaning Steps Performed

1. **Removed duplicate rows** to ensure data integrity.
2. **Dropped irrelevant columns** that provided no analytical value.
3. **Standardized key columns:**
   - `Last_Name`: Cleaned inconsistent formatting (e.g., extra spaces, non-alphabet characters).
   - `Phone_Number`: Formatted to a consistent pattern (e.g., (123) 456-7890).
4. **Handled missing values:**
   - Removed entries with `NaN` or `"N/a"` values.
   - Used **mode imputation** to fill missing values in categorical columns:
     - `Paying Customer`
     - `Do_Not_Contact`
5. **Split the dataset:**
   - `cleaned_data.xlsx`: Records with complete/non-null values.
   - `uncleaned_data.xlsx`: Records with null values (for transparency and auditing).
