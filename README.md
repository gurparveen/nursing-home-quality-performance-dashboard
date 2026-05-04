# 🏥 Nursing Home Quality & Performance Dashboard

**Nursing Home Quality &amp; Performance Dashboard — Excel Cleaning + Power BI Visualization (In Progress)**

This project analyzes **nursing home quality, staffing, ownership, and facility characteristics** using publicly available CMS datasets.
The goal is to build a **multi‑page Power BI dashboard** that provides clear insights into nursing home performance across the United States.

## 📌 Project Overview

This project follows a full analytics workflow:

1. **Excel** – Data cleaning, standardization, and quality checks  
2. **Power BI** – Data modeling and dashboard development  
3. **Dashboard Pages** (in progress):
    - ✔ **Overview Page** (Completed)
    - ⏳ Quality Page (In Progress)
    - ⏳ Staffing Page (In Progress)
    - ⏳ Facility Page (In Progress)
    - ⏳ Chain Ownership Page (In Progress)

## 📊 Completed: Overview Page

The Overview page includes:
- **Total Facilities**
- **Average Overall Rating**
- **Average Staffing Rating**
- **Average Residents per Day**
- **Facility Rating Distribution**
- **Ownership Breakdown**
- **Facility Size Distribution**
- **Geographic Distribution (Filled Map)**

📸 Screenshot
![Overview Page]()

## 🧹 Excel Data Cleaning

Cleaning steps performed:
- Removed duplicates
- Standardized column names
- Fixed inconsistent state codes
- Converted ratings to numeric
- Cleaned ownership categories
- Created cleaned_data.xlsx for Power BI import

## 📈 Power BI Development

- Built data model using cleaned Excel dataset
- Created DAX measures for ratings, counts, and averages
- Designed Overview page layout
- Added navigation sidebar for multi‑page experience
- Additional pages will be added as they are completed

## 🚧 Project Status: In Progress

This repository will be updated as each dashboard page is completed.

**Next steps:**
- Build Quality page (ratings, deficiencies, inspection trends)
- Build Staffing page (HPRD, RN hours, staffing ratings)
- Build Facility page (beds, occupancy, resident characteristics)
- Build Chain page (corporate ownership analysis)

## 🛠 Tools Used

**Excel** – Data cleaning & preparation  
**Power BI** – Dashboard design & modeling  
**GitHub** – Version control & portfolio hosting  

## 📁 Repository Structure

And include this:
```
nursing-home-quality-dashboard/
│
├── data/
│   ├── raw_cms_data.csv
│   └── cleaned_data.xlsx
│
├── excel-cleaning/
│   └── cleaning_steps.xlsx
│
├── powerbi/
│   └── nursing_home_dashboard.pbix
│
├── images/
│   └── overview_page.png
│
└── README.md
```

## 📬Contact

If you’d like to discuss this project or my analytics work, feel free to reach out.
