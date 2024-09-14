# Store Sales and Profit Analysis using Python

## Problem Statement

Analyzing the sales and profit performance of a retail store is crucial for businesses aiming to optimize operations, refine pricing strategies, enhance marketing efforts, and improve inventory management. This project leverages data-driven insights to identify areas for improvement and drive revenue and growth. It involves comprehensive analysis of store sales and profits using Python.

## Dataset

The dataset used for this analysis can be accessed via the following link:
[Download Dataset](https://drive.google.com/drive/folders/13v8yNFFFQ75RlgyyueIHZlrVX6QcRSet?usp=sharing)

## Key Components

### Data Preparation

1. **Converting Date Columns**: Transform date columns to datetime format to extract valuable time-based insights.
2. **Handling Missing Values and Outliers**: Prepare the dataset for analysis by managing missing values and outliers.

### Sales Analysis

1. **Temporal Sales Trends**: Analyze monthly sales patterns to inform inventory planning and promotional strategies.
2. **Category and Sub-Category Analysis**: Identify top-performing product categories and sub-categories to prioritize stock and refine product offerings.

## Getting Started

### Prerequisites

Ensure you have the following libraries installed:
- `pandas`
- `matplotlib`
- `seaborn`

You can install them using pip:
```bash
pip install pandas matplotlib seaborn
Running the Analysis
1.Upload the Dataset

Update the dataset file path in the code or use the file upload functionality to upload your dataset directly.

2.Load and Prepare Data

import pandas as pd
from google.colab import files

# Upload the dataset file
uploaded = files.upload()

# Read the uploaded dataset, specifying an encoding that handles non-UTF-8 files
df = pd.read_csv(list(uploaded.keys())[0], encoding='ISO-8859-1')

# Display the first few rows of the dataset
df.head()


3.Data Preparation

Convert date columns, handle missing values, and manage outliers.

4.Sales Analysis

Perform the following analyses:

Monthly Sales Trends
Category Performance
Sub-Category Performance
Profitability Analysis
Example code snippets are provided in the accompanying Python scripts.

Example Analysis
Here are some example analyses that you can perform:

Monthly Sales Trends

# Group by year and month to get monthly sales
monthly_sales = df.groupby(['Year', 'Month'])['Sales'].sum().reset_index()


Category Performance

# Group by Category to analyze the total sales by category
category_sales = df.groupby('Category')['Sales'].sum().reset_index()

Profitability Analysis

# Group by year and month to get monthly profit
monthly_profit = df.groupby(['Year', 'Month'])['Profit'].sum().reset_index()
