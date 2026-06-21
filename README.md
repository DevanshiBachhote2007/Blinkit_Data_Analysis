# Blinkit Data Analysis

[![Open Notebook](https://img.shields.io/badge/Open-Blinkit_data_analysis.ipynb-blue?style=for-the-badge)](Blinkit_data_analysis.ipynb) [![Open CSV File](https://img.shields.io/badge/Open-blinkit_data.csv-lightgrey?style=for-the-badge)](blinkit_data.csv)

## Table of Contents
- Project Overview
- Executive Summary
- Problem Statement
- Dataset Explanation
  - Dataset fields
  - Data cleaning step
- Technical Stack
- Quick Start
  - Prerequisites
  - Run the analysis
- Project Structure
- Visual Preview
- Key Insights
- Author

  
## 📌 Project Overview
This repository contains the `Blinkit_data_analysis.ipynb` notebook, which performs exploratory data analysis on the Blinkit retail dataset using Python. The analysis covers data cleaning, KPI calculations, visualizations, and key insights to help inform merchandising and outlet strategy.

## 📈 Executive Summary
The notebook analyzes 8,523 Blinkit records and reveals these main findings:
- **Low Fat items generate the highest total sales** after cleaning fat content categories.
- **Fruits and Vegetables, Snack Foods, and Household products** are top-selling item types.
- **Outlet Location Type and Size strongly influence sales**, with medium outlets and Tier 1 / Tier 3 stores contributing significantly.
- **Outlet Establishment Year** shows sales trends that can guide expansion planning.

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

###  Dataset fields
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
<img width="572" height="476" alt="image" src="https://github.com/user-attachments/assets/377bca06-57bd-4aa2-abb8-40517f8246f0" />

### Sales by Item Type
<img width="1058" height="591" alt="image" src="https://github.com/user-attachments/assets/900ca85c-ce2f-4be1-bb4a-1707cec2b42a" />


### Sales by Outlet Location Type and Fat Content
<img width="854" height="483" alt="image" src="https://github.com/user-attachments/assets/9e0fcf59-2112-4902-ba90-5c313b1c9ff9" />


### Sales by Outlet Establishment Year
<img width="937" height="506" alt="image" src="https://github.com/user-attachments/assets/87ad060f-3d28-4aa0-8f54-b58a97e2f36b" />


### Sales Distribution by Outlet Size
<img width="398" height="379" alt="image" src="https://github.com/user-attachments/assets/71e0bbe3-94a2-4993-bf9f-21f6ff4eaed9" />


### Sales by Outlet Location Type
<img width="859" height="297" alt="image" src="https://github.com/user-attachments/assets/75195404-53da-4f5f-baa0-03af097fea4f" />


## ✅ Key Insights
- `Low Fat` products show the strongest sales share after data cleaning.
- `Fruits and Vegetables` is the highest-earning product category.
- Medium outlets are the most valuable by total sales.
- Outlet location and establishment year both matter for revenue strategy.

## ✍️ Author
- Devanshi Bachhote

