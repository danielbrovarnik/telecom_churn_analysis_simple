# telecom_churn_analysis_simple


# Create a README.md file with the content provided earlier

readme_content = """
# Customer Churn Analysis by Tenure and Contract Type

This project analyzes the relationship between customer churn, contract type, and tenure using the **Telco Customer Churn** dataset.

## Overview

The goal is to visualize how churn rates vary based on:
- **Customer tenure (in months)**
- **Type of contract** (e.g., Month-to-month, One year, Two year)

A heatmap is created to highlight patterns and trends in churn rates.

## Dataset

**File used:** `WA_Fn-UseC_-Telco-Customer-Churn.csv`  
This dataset includes customer information from a fictional telecom company, including whether the customer churned, their contract type, and how long they've been with the company.

## Process

1. **Load and Preview Data**  
   The dataset is loaded using pandas and the first few rows are displayed to understand its structure.

2. **Select Relevant Features**  
   Extracts only the necessary columns: `tenure`, `Contract`, and `Churn`.

3. **Data Cleaning**  
   Checks for missing values in the selected columns.

4. **Feature Engineering**  
   Converts the categorical `Churn` column into a numeric format (`Churn_numeric`), where:
   - `1` represents a churned customer
   - `0` represents a retained customer

5. **Group and Aggregate**  
   Groups data by `tenure` and `Contract` and calculates the **average churn rate** for each combination.

6. **Visualization**  
   Creates a heatmap using Seaborn to show churn rates across different tenure values and contract types.

## Output

The output is a heatmap with:
- **X-axis:** Tenure (in months)
- **Y-axis:** Contract Type
- **Color scale:** Average churn rate (darker = higher churn)
  ![image](https://github.com/user-attachments/assets/2c539b7f-5b06-402b-a096-48bbc4a23dd9)


## Requirements

Make sure to install the following Python packages:
```bash
pip install pandas seaborn matplotlib
