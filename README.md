# Data Quality Project – Online Retail Dataset

This repository contains my data quality project using the Online Retail Dataset.  
In this project, I focused on checking different data quality issues using the concepts 
from data warehousing and data mining. The goal was to understand the problems in the data 
and prepare it for further analysis.

## 📁 Files in This Repository
- **OnlineRetailDataQuality.ipynb** – My complete analysis in a Colab notebook  
- **results/** – Folder that contains all charts, tables, and CSV files I generated  
- **README.md** – Project explanation  
- **data.zip** – Compressed file containing the dataset  

## 📊 Dataset Information
Source of the dataset :  
https://archive.ics.uci.edu/dataset/316/online+retail

The dataset has around **541,909 rows** with these columns:
InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country.

## 🔍 What I Did in This Project
I checked the data using three important data quality dimensions:

### ✔ Completeness
- Missing CustomerID (~135k missing)  
- Missing Description (~1.4k missing)

### ✔ Validity
- Negative quantities  
- Zero or negative UnitPrice  
- Unusual StockCodes (non-numeric)  
- Verified that InvoiceDate values were valid  

### ✔ Consistency
- Duplicate rows  
- Same StockCode appearing with multiple descriptions  
- Cancelled invoices (InvoiceNo starting with “C”)  
- Outliers in Quantity and UnitPrice  

All the results from these checks are available in the **results/** folder.

## 🛠 Tools I Used
- Python (Pandas, NumPy)  
- Google Colab  
- GitHub  

## ▶ How to Run This Notebook
Download the data.zip file from this repository and extract it. 
After extracting, make sure the file is named data.csv and place it in the same folder as the notebook. 
Then open the notebook in Google Colab or Jupyter Notebook and run the cells in order.


## 📌 Note
This repository contains all the files used and generated during my data quality project.
