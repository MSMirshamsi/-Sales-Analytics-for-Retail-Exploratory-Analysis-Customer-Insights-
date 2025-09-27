# Sales Analytics for Retail — Exploratory Analysis & Customer Insights  
**Data:** `sales.xlsx` (realistic retail invoices)  
**Tech stack:** `Python`, `pandas`, `numpy`, `matplotlib`, `seaborn` (Jupyter Notebook)

---

## 🚀 Project Summary (one-liner)
A focused, business-driven sales analysis pipeline on invoice-level data (provided as `sales.xlsx`) delivering actionable insights: data cleaning, EDA, market performance, RFM customer segmentation, and customer retention analysis — all implemented in a production-ready Jupyter notebook.

---

## 🎯 Why this project matters
Retail organizations routinely rely on Excel exports. This project shows how to transform raw invoice files into clean, analyzable data and produce business intelligence that supports marketing, sales strategy, and retention programs. It demonstrates practical SQL-free data engineering, robust EDA, customer lifetime insights, and easy-to-interpret visual storytelling — skills hiring managers look for in Data Analysts and BI specialists.

---

## 📦 Dataset (provided)
File: `sales.xlsx` (included in the repository)

**Columns / Description**
- `InvoiceNumber` — 6-character invoice id (starts with `C` for cancelled invoices)  
- `ProductCode` — 5-digit code for the product  
- `ProductName` — product title  
- `Quantity` — quantity of product in the invoice row  
- `InvoiceDate` — invoice creation datetime  
- `UnitPrice` — unit price of the product  
- `CustomerId` — 5-digit customer id  
- `Country` — customer country

> Note: The notebook contains data validation and robust parsing to handle possible inconsistencies in the Excel file.

---

## 🧭 Project workflow (5 stages)
1. **Data preprocessing**  
   - Load Excel safely; handle corrupt / malformed files.  
   - Parse datetimes, normalize column names, drop duplicates, handle cancellations (`InvoiceNumber` starting with `C`), and derive `TotalPrice = Quantity * UnitPrice`.  

2. **Exploratory Data Analysis (EDA)**  
   - Descriptive statistics (sales distribution, price, quantity).  
   - Key visualizations: revenue over time, top products, top customers, product price distributions, cancellations.  

3. **Market / Geographic study**  
   - Country-level sales vs. customer counts — identify markets with high customer counts but low revenue (opportunities for up-sell / pricing adjustments).  
   - Visual maps / bar charts and ratio metrics (Revenue per Customer).  

4. **Customer valuation: RFM segmentation**  
   - Compute **R**ecency, **F**requency, **M**onetary for each customer.  
   - Score and cluster customers into 7 business-meaningful segments (VIP, Loyal, At-Risk, New, Occasional, Discount-Seeking, Churned).  
   - Provide marketing recommendations per segment (campaign suggestions & expected KPIs).

5. **Customer retention analysis**  
   - Cohort analysis to estimate retention over months after customers’ first purchase.  
   - Compute percent of customers who make repeat purchases by month; visualize cohort retention heatmap.

---

## ✅ Key deliverables (in the notebook)
- `01_preprocessing.ipynb` (or first notebook cell): robust loading & cleaning of `sales.xlsx`.  
- EDA charts (time-series revenue, top products/customers).  
- Market opportunity tables (country revenue vs. unique customers).  
- RFM build & segmentation (scoring logic + table of segments).  
- Retention / cohort analysis and visualizations.  
- A final summary: top 5 business recommendations.

---

## 📈 Business impact & insights (examples)
- Identifies top-10 revenue-driving products and customers for targeted account management.  
- Detects markets with many customers but low average order value — immediate marketing / pricing interventions.  
- Segments customers to support tailored campaigns: e.g., “win-back” for At-Risk customers, loyalty offers for VIPs.  
- Quantifies monthly retention rates to measure customer lifetime growth.

---

## 🛠️ Skills & techniques demonstrated
- Data ingestion and robust Excel parsing (recovering from malformed Excel files).  
- Time-series aggregation and trend detection.  
- Grouping, aggregation, pivoting with `pandas`.  
- Window-like analyses using `groupby` and `rolling` logic.  
- RFM calculation and rule-based segmentation.  
- Cohort/retention analysis and heatmap visualization.  
- Clean, well-documented Jupyter Notebook suitable for review by hiring managers.

---
