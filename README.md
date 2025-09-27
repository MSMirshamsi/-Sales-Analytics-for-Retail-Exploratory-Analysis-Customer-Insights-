# Apple Sales Data Analysis

## Project Overview
This project is an **end-to-end data analysis case study** based on a transactional sales dataset from **Apple Inc. (simulated)**.  
The goal is to demonstrate professional **data analytics techniques** using **Python, Pandas, NumPy, Matplotlib, and Seaborn**.

The dataset contains detailed transactional data such as:
- `InvoiceNumber` → Unique 6-digit invoice (prefix **C** = cancelled order)  
- `ProductCode` → Unique 5-digit product identifier  
- `ProductName` → Item description  
- `Quantity` → Number of units per transaction  
- `InvoiceDate` → Date of transaction  
- `UnitPrice` → Price per unit  
- `CustomerId` → Unique 5-digit customer ID  
- `Country` → Customer location  

This analysis replicates the workflow of a **Data Analyst in a retail/tech company**, focusing on **customer insights, revenue patterns, and market behavior**.

---

## Objectives
The project is structured into **five main analytical steps**:

1. **Data Preprocessing**
   - Handling missing values & duplicates  
   - Standardizing column names  
   - Managing cancelled invoices (InvoiceNumber starting with `C`)  
   - Parsing dates and extracting time-based features (month, year, etc.)  

2. **Exploratory Data Analysis (EDA)**
   - General trends in sales volume & revenue  
   - Identifying top-selling products  
   - Highlighting top customers and cancelling customers  
   - Visualizing seasonality and demand patterns  

3. **Market Analysis**
   - Ranking countries by sales volume  
   - Finding markets with high customer base but low revenue  
   - Visualizing global distribution of Apple’s sales  

4. **Customer Value Segmentation (RFM Analysis)**
   - Using **Recency, Frequency, Monetary** metrics  
   - Clustering customers into **7 behavioral groups**  
   - Extracting insights into VIP customers, churn risks, and regular buyers  

5. **Customer Retention Analysis**
   - Measuring repeat purchase rate  
   - Month-to-month retention visualization  
   - Identifying loyalty trends and growth opportunities  

---

## Techniques & Tools Used
- **Data Wrangling & Cleaning** → `pandas`, `numpy`  
- **Exploratory Data Analysis (EDA)** → grouping, aggregations, pivot tables  
- **Visualization** → `matplotlib`, `seaborn` (heatmaps, bar charts, time-series plots)  
- **Customer Segmentation (RFM Model)** → quantile-based classification into customer tiers  
- **Retention Analysis** → cohort analysis using invoice dates  
- **Business Insights** → identifying revenue leaks, growth markets, and key customer groups  

---

## Example Visuals
The notebook generates various charts, including:  
- Monthly sales trend with cancellations highlighted  
- Top 10 best-selling Apple products  
- Country-wise sales performance (bar and map-style charts)  
- RFM distribution plots (Recency vs. Frequency vs. Monetary)  
- Customer retention curves  

---

