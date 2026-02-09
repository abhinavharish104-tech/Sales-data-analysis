# Sales Data Cleaning and Analysis Using Pandas

### A mini data analytics project demonstrating end-to-end data preprocessing, analysis, and visualization with Python.

---

##  Project Overview

Real-world datasets are rarely clean. This project focuses on transforming a messy retail sales dataset into a structured, analysis-ready format using **Pandas**, followed by exploratory analysis and visualization.

### The objective was to:

- Detect and handle missing values  
- Remove duplicate records  
- Standardize column formatting  
- Generate meaningful summaries  
- Create insightful visualizations  
- Save a cleaned dataset for further use  

---

##  Dataset Description

The dataset (**sales_data.csv**) contains raw sales records with the following columns:

- Customer Name  
- Product  
- Quantity  
- Price  
- Sale Date  
- Region  

### Data Quality Issues

The original dataset included:

- Missing values in several columns  
- Duplicate entries  
- Inconsistent column names  
- Unstructured formatting  

These issues were addressed systematically through data cleaning steps.

---

##  Tools & Technologies

- **Python 3**  
- **Pandas** – data cleaning and manipulation  
- **Matplotlib & Seaborn** – visualization  
- **Jupyter Notebook** – development environment  

---

##  Data Cleaning Process

The following steps were performed to prepare the dataset:

### 1. Data Loading and Inspection

- CSV file imported using `pandas.read_csv()`  
- Dataset explored using `head()`, `info()`, and `isnull()`  

### 2. Handling Missing Values

- Numerical columns (`quantity`, `price`)  
  - Filled with their respective mean values  

- Categorical columns (`customer_name`, `region`)  
  - Filled with **"Unknown"**

- Date column (`sale_date`)  
  - Filled with the most frequent date  

- Missing value patterns visualized using a heatmap  

### 3. Removing Duplicates

- Duplicate rows identified and removed  
- Only the first occurrence of repeated records retained  

### 4. Column Standardization

- Column names converted to lowercase  
- Spaces replaced with underscores  

Example:

Customer Name → customer_name


### 5. Feature Engineering

- New column created:

total_sale = quantity × price


- Numerical columns rounded for better readability  

### 6. Export Cleaned Dataset

- Final dataset saved as:

sales_data_cleaned.csv


---

##  Exploratory Data Analysis

After cleaning, multiple analyses were performed.

### Visualizations Created

- Missing Value Heatmap  
- Sales Volume by Region  
- Average Price by Region  
- Top 3 Best-Selling Products  
- Sales Trend Over Time  
- Price Distribution  
- Correlation Matrix  

These visuals helped convert raw numbers into actionable insights.

---

##  Key Insights

From the analysis, the following conclusions were drawn:

- All missing values were successfully handled  
- Certain regions generated higher sales volumes  
- A small number of products contributed most of the sales  
- Sales performance varied noticeably across dates  
- Quantity and price both strongly influenced total revenue  

---

##  Project Deliverables

This repository contains:

- **sales_data.csv** – Original raw dataset  
- **sales_data_cleaned.csv** – Cleaned and processed dataset  
- **sales_analysis.ipynb** – Jupyter Notebook with code and visualizations  
- **README.md** – Project documentation  

---

###  End-to-end project completed using Python and Pandas.
