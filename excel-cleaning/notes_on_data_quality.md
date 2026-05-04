## 1. Overview  

This document summarizes the data quality issues identified in the CMS Nursing Home dataset and the steps taken to ensure accuracy before analysis and dashboard development. The dataset was generally clean, with only formatting and consistency issues requiring correction.

## 2. Data Source Notes

- Source: CMS Nursing Home – General Information dataset
- Approx. 15,000 facilities across the United States
- The CMS Nursing Home dataset is not fully clean. It contains several formatting issues, missing values, inconsistent categories, and data type problems. Only partial cleaning is applied by CMS, so additional cleaning steps were required before analysis.

## 3. Data Quality Issues Identified

### Missing or Null Values

- Some facilities have missing ratings (Overall, Staffing, Quality)
- A few facilities have missing resident census values
- Ownership category missing for a small subset

### Inconsistent Formats

- **ZIP Codes stored as numbers instead of text**, causing leading zeros to drop
  - Example: 07086 → 7086
  - Some ZIPs appear with only 3 digits due to formatting

- State codes appear in mixed case (e.g., ny, NY, Ny)
- Ownership categories inconsistent (e.g., “For Profit”, “For‑Profit”, “for_profit”)

### Data Type Problems

- Ratings imported as text instead of numeric
- Resident counts imported as text
- Some numeric fields imported as “General”

### Duplicates

- Occasional duplicate facility names or addresses
- Rare duplicate provider IDs

### Outliers

No statistical outliers were found in the dataset. All numeric fields (ratings, resident counts, bed counts) fell within expected CMS ranges.
Only formatting issues (such as ZIP code length) appeared unusual but were not outliers.

## 4. Assumptions Made

No assumptions were made during the cleaning process.
All values were kept exactly as provided by CMS.
Only formatting corrections (such as fixing ZIP code length issues) were applied.

## 5. Data Cleaning Actions Taken

- Standardized column names
- Converted rating fields to numeric
- Cleaned and grouped ownership categories
- Corrected ZIP Codes by restoring leading zeros and converting to text
- Fixed inconsistent state codes
- Removed exact duplicate rows
- Created cleaned_data.xlsx for Power BI import

## 6. Limitations

The CMS dataset is generally clean. Some fields contain missing values (ratings, resident counts, ownership), which may affect certain averages or visualizations.

## 7. Recommendations for Future Improvements

Future enhancements may include adding historical CMS data to analyze trends over time or combining additional CMS datasets for deeper insights.
