# Blinkit Data Analysis

[![Open Notebook](https://img.shields.io/badge/Open-Blinkit_data_analysis.ipynb-blue?style=for-the-badge)](Blinkit_data_analysis.ipynb) [![Open CSV File](https://img.shields.io/badge/Open-blinkit_data.csv-brightgreen?style=for-the-badge)](blinkit_data.csv)

## 📌 Project Overview
This repository contains the `Blinkit_data_analysis.ipynb` notebook, which performs exploratory data analysis on the Blinkit retail dataset using Python. The analysis covers data cleaning, KPI calculation, and visualizations that highlight sales patterns across item categories, outlet attributes, and fat-content segments.

## 📈 Executive Summary
The notebook analyzes 8,523 Blinkit records and reveals these main findings:
- **Low Fat items generate the highest total sales** after cleaning fat content categories.
- **Fruits and Vegetables, Snack Foods, and Household products** are top-selling item types.
- **Outlet Location Type and Size strongly influence sales**, with medium outlets and Tier 1 / Tier 3 stores contributing significantly.
- **Outlet Establishment Year** shows sales trends that can guide expansion planning.

## 📚 Table of Contents
- [Project Overview](#📌-project-overview)
- [Executive Summary](#📈-executive-summary)
- [Problem Statement](#⚠️-problem-statement)
- [Dataset Explanation](#📊-dataset-explanation)
- [Technical Stack](#🛠️-technical-stack)
- [Quick Start](#🚀-quick-start)
- [Project Structure](#📂-project-structure)
- [Key Insights](#✅-key-insights)
- [Author](#✍️-author)

## ⚠️ Problem Statement
This analysis answers key business questions such as:
- Which fat-content category contributes most to sales?
- Which product types drive the largest revenue?
- How do outlet location, size, and establishment year relate to total sales?
- What operational patterns can Blinkit use for store planning and product focus?

## 📊 Dataset Explanation
- **Dataset file:** `blinkit_data.csv`
- **Rows:** 8,523
- **Columns:** 12
- **Missing values:** only `Item Weight` contains missing data (1,463 rows)

### Dataset fields
- `Item Fat Content` — categorical food fat label (Regular, Low Fat, LF, low fat, reg)
- `Item Identifier` — unique item code
- `Item Type` — product category (e.g. Fruits and Vegetables, Dairy, Snack Foods)
- `Outlet Establishment Year` — year the store opened
- `Outlet Identifier` — unique store ID
- `Outlet Location Type` — tiered area classification (Tier 1, Tier 2, Tier 3)
- `Outlet Size` — store size (Small, Medium, High)
- `Outlet Type` — business format type (Supermarket Type1, Grocery Store, etc.)
- `Item Visibility` — display visibility metric
- `Item Weight` — product weight
- `Sales` — revenue metric used for KPI and visual analysis
- `Rating` — customer rating score

### Data cleaning step
- Standardized `Item Fat Content` values by replacing:
  - `LF` → `Low Fat`
  - `low fat` → `Low Fat`
  - `reg` → `Regular`

## 🛠️ Technical Stack
- Python 3.x
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn

## 🚀 Quick Start
### Prerequisites
- Python 3.x installed
- Jupyter Notebook or VS Code with Jupyter extension

### Run the analysis
```bash
pip install pandas numpy matplotlib seaborn
jupyter notebook
```
Open `Blinkit_data_analysis.ipynb` and run the cells sequentially.

## 📂 Project Structure
```
Python/
├── Blinkit_data_analysis.ipynb
├── README.md
└── blinkit_data.csv
```

## 💡 Visual Preview
### Sales by Fat Content
![Sales by Fat Content](images/sales_by_fat.png)

### Sales by Item Type
![Sales by Item Type](images/sales_by_item_type.png)

### Sales by Outlet Location Type and Fat Content
![Fat Content by Outlet](images/fat_content_by_outlet.png)

### Sales by Outlet Establishment Year
![Sales by Outlet Year](images/sales_by_outlet_year.png)

### Sales Distribution by Outlet Size
![Sales by Outlet Size](images/sales_by_outlet_size.png)

### Sales by Outlet Location Type
![Sales by Outlet Location](images/sales_by_outlet_location.png)

## ✅ Key Insights
- `Low Fat` products show the strongest sales share after data cleaning.
- `Fruits and Vegetables` is the highest-earning product category.
- Medium outlets are the most valuable by total sales.
- Outlet location and establishment year both matter for revenue strategy.

## ✍️ Author
- Your Name Here
