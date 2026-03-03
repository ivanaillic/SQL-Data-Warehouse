# 📦 SQL Data Warehouse Project (SQL Server)

End-to-end Data Warehouse implementation built in Microsoft SQL Server using a Medallion Architecture (Bronze → Silver → Gold).  
The project integrates CRM and ERP datasets and delivers an analytics-ready Star Schema.

---

## 🎯 Project Objective

- Integrate multiple source systems (CSV files)  
- Clean and standardize raw data  
- Apply business transformation rules  
- Deliver a reporting-ready data model  
- Ensure data integrity through quality validation  

---

## 🏗 Architecture

### 🥉 Bronze Layer

- Raw CSV ingestion using `BULK INSERT`  
- Batch loading via stored procedure  
- Truncate-and-load strategy with logging and error handling  

### 🥈 Silver Layer

- Data cleansing and standardization  
- Validation of keys, dates, and financial consistency  
- Business rule implementation  
- Cross-source integration  

### 🥇 Gold Layer

- Star Schema implemented as SQL views  
- `dim_customers`, `dim_products`, `fact_sales`  
- Surrogate keys generated via `ROW_NUMBER()`  
- Referential integrity checks  

---

## 🛠 Tech Stack

- Microsoft SQL Server    
- Stored Procedures  
- Star Schema Modeling  
