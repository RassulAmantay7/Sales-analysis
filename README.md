# Optimizing Retail Strategy through Sales Data Exploration

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-444444)

## 📌 Project Overview
This project performs an end-to-end Exploratory Data Analysis (EDA) on supermarket sales data. By analyzing transaction patterns across different product lines and demographics, the study identifies specific peak sales periods and consumer behaviors to help supermarket management optimize inventory and marketing efforts.

## 📊 Dataset
The dataset represents historical sales of a supermarket company which has been recorded in 3 different branches for 3 months.
* **Source:** [Kaggle - Supermarket Sales Dataset](https://www.kaggle.com/datasets/akashbommidi/super-market-sales)
* **Key Attributes:** Customer segmentation, Product lines, Gender, Payment methods, and Gross Income.

## 🛠️ Data Cleaning & Feature Engineering
Before analysis, the data underwent the following preprocessing steps:
* **Handling Irrelevant Data:** Removed `Invoice ID` and `Branch` to focus on global sales trends.
* **DateTime Transformation:** Converted the `Date` column to datetime objects.
* **Temporal Feature Extraction:** Extracted the "Day of the Week" to analyze weekday vs. weekend performance.
* **Categorical Ordering:** Established a chronological order for weekdays (Monday-Sunday) to ensure logical visualizations.

## 📈 Key Insights

### 1. Gender-Based Revenue Analysis
* **Observation:** Analyzed the correlation between Gender and Gross Income.
* **Insight:** Identified which product categories are dominated by specific genders, allowing for more targeted promotional campaigns.

### 2. Temporal Product Performance (Facet Analysis)
* **Visual Method:** Used a Seaborn `FacetGrid` to visualize every Product Line's performance across the week.
* **Strategic Findings:** * **Electronic accessories:** Peak performance occurs on **Thursdays**.
    * **Home and lifestyle & Fashion accessories:** Show significant spikes during **weekends**.
    * **Health and beauty:** Sales remain relatively stable but show unique mid-week trends.



## 💡 Recommended Strategies
* **Dynamic Stocking:** Increase inventory for "Fashion" and "Home" categories on Friday evenings to prepare for weekend surges.
* **Weekday Promotions:** Launch "Tech Thursdays" with specific discounts on Electronic accessories to capitalize on existing consumer trends.
* **Gender-Targeted Marketing:** Align store layouts to highlight high-income categories specific to the demographic peaks identified in the data.

## 📂 Repository Structure
```text
├── data/
│   └── supermarket_sales.csv   # Raw dataset (Ignored by Git)
├── notebooks/
│   └── Optimizing Retail Strategy through Sales Data Exploration.ipynb
├── .gitignore                  # Standard DS gitignore
└── README.md                   # Project documentation