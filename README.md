# 📊 Finnish Political Party Financing & Campaign Expenses (2023–2025)

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Data_Modeling-blue?style=for-the-badge)
![Power Query](https://img.shields.io/badge/Power_Query-ETL-green?style=for-the-badge)

## 📌 Project Overview
An end-to-end Business Intelligence & Data Analytics project evaluating financial disclosures, election campaign expenditures, state subsidies, workforce costs, and private donations across Finland's 5 major political parties during the **2023–2025 electoral cycle**.

📄 **Executive Analytics Report:** [Download Executive PDF Report](./powerbi/Finnish_Party_Financing_Executive_Report.pdf)  
📊 **Dashboard PDF Export:** [Download Dashboard PDF](./powerbi/Finland_Political_Parties_BI_Dashboard.pdf)

---

## 📂 Repository Structure
```text
├── README.md
├── data_processed/                                   # Cleansed & Merged Excel Workbooks
│   ├── CampaignExpenses_2023-2025.xlsx
│   ├── Donations_2023-2025.xlsx
│   ├── Financials_2023-2025.xlsx
│   ├── HR_Expenses_2023-2025.xlsx
│   ├── PartyGrants_2023-2025.xlsx
│   ├── StateSupport_Transfers_2023-2025.xlsx
│   └── StateSupport_Use_2023-2025.xlsx
├── data_raw/                                         # Raw Financial Disclosures (Zipped by Party)
│   ├── kokomus.zip
│   ├── perussuomalaiset.zip
│   ├── sdp.zip
│   ├── suomen_keskusta.zip
│   └── vihrea_liitto.zip
└── powerbi/                                          # BI Assets & Executive Reports
    ├── Finland_Political_Parties_BI_Dashboard.pbix   # Interactive Power BI File
    ├── Finland_Political_Parties_BI_Dashboard.pdf    # Visual Dashboard Export
    └── Finnish_Party_Financing_Executive_Report.pdf  # Final Executive Analytics Report

## 💡 Key Metrics & Financial Insights

**General Financial Summary (2023–2025):**
- **Total Campaign Expenses:** **€29.37M** across 5 major parties over 3 years
- **Total State Support Use:** **€63.58M** in parliamentary operational grants
- **Total Private Donations:** **€4.22M** in corporate & individual contributions
- **Total HR Expenses:** **€27.16M** in workforce and organizational operations

**Campaign Spending Allocation by Party:**
- **Perussuomalaiset r.p.:** **€12.69M** (43.2%) — Peak spend in Municipal & Regional Elections 2025 (**€5.03M**)
- **Kansallinen Kokoomus r.p.:** **€6.81M** (23.2%) — Peak spend in Parliamentary Elections 2023 (**€1.62M**)
- **Suomen Sosialidemokraattinen Puolue r.p.:** **€4.63M** (15.8%) — Peak spend in Parliamentary Elections 2023 (**€2.08M**)
- **Suomen Keskusta r.p.:** **€2.97M** (10.1%) — Peak spend in Parliamentary Elections 2023 (**€1.81M**)
- **Vihreä liitto r.p.:** **€2.27M** (7.7%) — Peak spend in Parliamentary Elections 2023 (**€0.99M**)

---

## 🛠️ Data Pipeline & Technical Architecture

- **ETL & Data Transformation (Power Query):** Extracted raw party financial disclosures from `data_raw/`. Cleaned numeric data types and explicitly removed summary rows (`KULUT YHTEENSÄ`) to prevent double-counting.
- **Data Modeling:** Designed a Star Schema linking Fact tables (`Campaign Expenses`, `Donations`, `HR Expenses`, `State Support`) to Date and Party Dimension tables.
- **DAX Measures:** Structured explicit calculations (`Total Campaign Expenses`, `Total State Support`, `Total HR Expenses`, `Total Donations`, `Total Financials`) in a dedicated measure group.
- **Dashboard UX & Visual Standards:** Applied Power BI's built-in *Accessible City Park* theme for high contrast accessibility, tuning font hierarchy, label placement, and visual container spacing.

---

## 👩‍💻 Author

**Oksana Kocherzhat**  
Junior Data Analyst (OAMK)  
📍 Finland  
🔗 LinkedIn: www.linkedin.com/in/oksana-kocherzhat-834518231
