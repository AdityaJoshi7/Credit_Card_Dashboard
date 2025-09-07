
# Credit Card Financial Dashboard

## Introduction
The **Credit Card Financial Dashboard** is a data analytics project designed to provide **real-time insights into credit card operations**. Using **SQL**, **Power BI**, and **DAX calculations**, this dashboard helps stakeholders monitor key performance metrics such as revenue, transactions, customer demographics, and delinquency rates.  

The project integrates customer and transaction data, processes it in SQL, and visualizes it in Power BI for **weekly performance tracking**.  

---

##  Table of Contents
1. [Project Objective](#project-objective)  
2. [Data Sources](#data-sources)  
3. [Database Setup](#database-setup)  
4. [Dashboard & Features](#dashboard--features)   
6. [Usage](#usage)  
7. [Key Insights](#key-insights)  
8. [Dependencies](#dependencies)  

---

##  Project Objective
To develop a **comprehensive weekly financial dashboard** that:  
- Tracks **revenue, transactions, and customer engagement**  
- Highlights **trends across age, income, geography, and card type**  
- Provides **WoW (Week-over-Week) comparisons**  
- Supports **data-driven decision-making**

---

##  Data Sources
The project uses multiple datasets (CSV files):  
- **`credit_card.csv`** – Credit card transaction and usage details  
- **`cust_add.csv`** – Customer demographic & address information  
- **`cc_add.csv`** – Additional credit card details  
- **`cust_detail`** – Created in SQL for customer demographics  

All data is imported into a MySQL database (`ccdb`).  

---

##  Database Setup
1. Create the database:
   ```sql
   CREATE DATABASE ccdb;
   ```

2. Create tables (`cc_detail`, `cust_detail`).  

3. Import data:
   ```sql
   LOAD DATA INFILE 'credit_card.csv' INTO TABLE cc_detail ...
   LOAD DATA INFILE 'cust_add.csv' INTO TABLE cust_detail ...
   ```

---

##  Dashboard & Features
The **Power BI Dashboard (`Credit Card Dashboard.pbix`)** provides:  
- **Revenue Analysis** (Fees, Transactions, Interest)  
- **Customer Segmentation** (Age, Income, Gender, Education, Marital Status)  
- **Card Performance** (Category-wise transactions & usage)  
- **Geographic Insights** (State-wise contribution)  
- **Activation & Delinquency Tracking**  
- **Week-over-Week KPIs**  


---

##  Usage
- Update SQL paths to your CSV locations.  
- Refresh Power BI to pull latest data.  
- Use dashboard slicers to analyze **Revenue, Transactions, Customer Segments, Geography, and Card Types**.  
- Export dashboard visuals to **PDF, Excel, or PowerPoint** for reporting.  

---

##  Key Insights
From **Week 53 (31st Dec)**:  
- Revenue increased by **28.8% WoW**  
- YTD Revenue: **$57M**  
- YTD Interest Earned: **$8M**  
- Transactions: **$46M**  
- Male customers generated **$31M revenue**, Female **$26M**  
- Blue & Silver cards contribute **93% of transactions**  
- **TX, NY, CA** contribute **68% of revenue**  
- Activation Rate: **57.5%**  
- Delinquency Rate: **6.06%**  

---

## Dependencies
- **SQL (MySQL 8.0+)**  
- **Power BI Desktop**  
- **DAX Calculations** (for grouping, KPIs, and WoW metrics)  
- **CSV Data Files**  

---
