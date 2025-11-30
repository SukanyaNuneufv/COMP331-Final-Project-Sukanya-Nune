# COMP331 Final Project – Data Quality Analysis (Online Retail Dataset)

This repository contains the full analysis for my COMP 331 final project. 
The objective of this project is to apply data warehousing and data quality concepts 
from Weeks 10–11 to evaluate the quality of the Online Retail dataset and 
identify issues related to completeness, validity, and consistency.

## 📁 Repository Contents
- **OnlineRetailDataQuality.ipynb** – Jupyter notebook containing the complete analysis
- **data.csv** – Online retail transactional dataset (download instructions below)
- **results/** – Output charts, tables, and summary files
- **README.md** – Project description and instructions

## 🗂 Dataset
The dataset used in this project can be downloaded from:
https://archive.ics.uci.edu/dataset/316/online+retail

After downloading, rename the file to **data.csv** and place it in the same folder 
as the notebook before running the analysis.

Rows: ~541,909  
Columns: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country

## 🔍 Analysis Summary
The notebook evaluates the dataset using:

### ✔ Completeness Checks  
- Missing CustomerID (~135K missing)  
- Missing Description (~1.4K missing)

### ✔ Validity Checks  
- Negative quantities (~10K rows)  
- Zero or negative UnitPrice (~2.5K rows)  
- Unusual alphanumeric StockCodes  
- Date value validity checks

### ✔ Consistency Checks  
- Duplicate rows  
- Same StockCode with multiple Descriptions  
- Canceled invoices (InvoiceNo starting with "C")  
- Outliers in Quantity and UnitPrice

## 🛠 Tools Used
- Python (Pandas, NumPy)
- Google Colab
- GitHub

## 📘 How to Run the Notebook
1. Download the `.ipynb` file
2. Download the dataset (link above)
3. Place `data.csv` in the same folder as the notebook
4. Run all code cells in Google Colab or Jupyter Notebook

## 📎 Course Requirement
This repository link is included in my final 2-page PDF report as required.
