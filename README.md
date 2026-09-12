# ✈️ Power BI Tourism Package Analysis Dashboard

## 📊 Project Overview

This Power BI project analyzes tourism/customer data to understand **tour package purchase behavior** across product types, contact channels, occupation, age groups, gender, and marital status.

The report is organized into focused analytical pages plus a summary page. KPI cards, pivot-style tables, donut charts, stacked-column analysis, and slicers are used to compare customers who took a package with those who did not.

## 🎯 Objectives

- Measure the total customer population.
- Compare customers who took a tourism package with those who did not.
- Analyze package purchase behavior by product pitch.
- Compare package outcomes by type of customer contact.
- Study package participation across occupations.
- Analyze package participation across age groups.
- Examine the effect of gender and marital-status filters on the report.

## 🛠️ Tools & Technologies

- **Microsoft Power BI Desktop**
- **Power Query** for data preparation/transformation
- **DAX** for calculated measures
- Interactive slicers, tables, charts, and KPI cards

## 🗂️ Data Model

The report uses the **`Tour_Data`** table.

Important fields used in the report include:

- `ProductPitched`
- `ProdTaken`
- `TypeofContact`
- `Occupation`
- `AGE_LABEL`
- `Gender`
- `MaritalStatus`

## 📌 Report Pages

### 1. Product Pitched

This page analyzes package-purchase behavior by the product that was pitched to the customer.

**Visuals used:**
- KPI card with:
  - `M_Total_Customers`
  - `M_Package_Taken`
  - `M_Package_Not_Taken`
  - `M_Contri`
- Pivot table using `ProductPitched`, `ProdTaken`, `M_Total_Customers`, and `M_%_Contri`.
- Donut chart for package taken by `ProductPitched`.
- `Gender` slicer.
- `MaritalStatus` slicer.

**Purpose:** Compare customer/package outcomes across product pitches and evaluate each product's contribution.

---

### 2. Type of Contact

This page focuses on the channel/type through which customers were contacted.

**Visuals used:**
- KPI card with the main package measures.
- Pivot table using `TypeofContact`, `ProdTaken`, `M_Total_Customers`, and `M_%_Contri`.
- Donut chart for package taken by `TypeofContact`.
- `Gender` slicer.
- `MaritalStatus` slicer.

**Purpose:** Understand how package outcomes vary according to the type of customer contact.

---

### 3. Occupation

This page compares package behavior across customer occupation categories.

**Visuals used:**
- KPI card with the main package measures.
- Pivot table using `Occupation`, `ProdTaken`, `M_Total_Customers`, and `M_%_Contri`.
- Donut chart for package taken by `Occupation`.
- `MaritalStatus` slicer.
- `Gender` slicer.

**Purpose:** Compare package participation among different occupation groups and examine their contribution to the overall customer/package mix.

---

### 4. Age

This page studies package behavior across predefined age groups.

The report uses the `AGE_LABEL` field and contains these age-group labels in the visual model:

- `Young`
- `Mid`
- `Old`
- `Sr`

**Visuals used:**
- KPI card with the main package measures.
- Pivot table using `AGE_LABEL`, `ProdTaken`, and `M_Total_Customers`.
- Donut chart for package taken by `AGE_LABEL`.
- 100% stacked column chart using `AGE_LABEL`, `M_Total_Customers`, and `ProdTaken`.
- `Gender` slicer.
- `MaritalStatus` slicer.

**Purpose:** Compare package uptake and customer distribution across age groups and see the relative composition of package outcomes.

---

### 5. Summary

This page consolidates the major dimensions used in the report for an overall comparison.

**Visuals used:**
- KPI card with the main package measures.
- Pivot table for `ProductPitched` vs `ProdTaken`.
- Pivot table for `TypeofContact` vs `ProdTaken`.
- Pivot table for `Occupation` vs `ProdTaken`.
- Pivot table for `AGE_LABEL` vs `ProdTaken`.
- `Gender` slicer.
- `MaritalStatus` slicer.

**Purpose:** Provide a compact summary view across product, contact type, occupation, and age, while keeping the key KPIs visible.

## 📏 DAX Measures Used

The report contains the following named measures:

| Measure | Purpose |
|---|---|
| `M_Total_Customers` | Total customer KPI used across the report |
| `M_Package_Taken` | KPI for customers who took the package |
| `M_Package_Not_Taken` | KPI for customers who did not take the package |
| `M_Contri` | Contribution KPI shown on the report cards |
| `M_%_Contri` | Contribution percentage used in the analytical tables |

## 🎛️ Interactive Filtering

The report uses the following slicers:

- **Gender**
- **MaritalStatus**

These filters are available on the analytical pages and the summary page.

## 📈 Visualization Techniques

- KPI Cards
- Pivot-style Tables
- Donut Charts
- 100% Stacked Column Chart
- Slicers

## 💡 Analytical Areas Covered

The dashboard connects multiple customer dimensions with package-purchase behavior:

**Product Pitched → Contact Type → Occupation → Age → Gender → Marital Status → Package Taken/Not Taken**

## 📂 Repository Contents

```text
PowerBI-Tourism-Analysis/
│
├── PowerBI_Tourism_Project.pbix
├── README.md
└── screenshots/
    └── tourism_dashboard.png
```

## 🚀 How to Use

1. Download `PowerBI_Tourism_Project.pbix`.
2. Open it using **Microsoft Power BI Desktop**.
3. Navigate through the five report pages.
4. Use the Gender and Marital Status slicers to change the analysis.
5. Interact with the tables and charts to explore package-purchase patterns.

## 🎓 Skills Demonstrated

- Power BI dashboard development
- Data analysis and visualization
- DAX measures
- Interactive filtering
- Customer segmentation
- Tourism package purchase analysis
- Comparative analysis across demographic and behavioral dimensions

## 👤 Project

**Power BI Tourism Package Analysis**
