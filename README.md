# Data-Warehouse-Big-query-and-power-bi
# 🏢 End-to-End Real Estate Data Platform & Analytics Solution

An end-to-end Data Engineering and Business Intelligence project built to process, model, and visualize real estate data using **Google BigQuery** and **Power BI**. The project follows the modern **Medallion Architecture (Bronze, Silver, Gold)** to ensure data reliability, scalability, and accurate reporting.

---

## 🏗️ Architecture & Pipeline (Medallion Architecture)

1. **Bronze Layer (Raw Data):** 
   - Ingested raw CSV files directly into Google BigQuery without any modifications to preserve a pristine historical record of the source data.
2. **Silver Layer (Data Transformation & Cleaning):** 
   - Cleaned and standardized raw data using advanced SQL queries. 
   - Handled data types casting (`SAFE_CAST`), parsed dates (`SAFE.PARSE_DATE`), managed missing values, trimmed whitespaces (`TRIM`), and filtered out null primary keys.
3. **Gold Layer (Star Schema & Data Modeling):** 
   - Designed a robust **Star Schema** consisting of **1 Fact Table** (capturing individual sale transactions) and **6 Dimension Tables** (`dim_project`, `dim_unit`, `dim_customer`, `dim_broker`, `dim_campaign`, and `dim_date`).
   - Strictly enforced **One-to-Many (1 to *) relationships** to prevent data ambiguity and calculation errors.

---

## 🛠️ Tech Stack & Tools
* **Data Warehouse & ETL:** Google BigQuery (SQL)
* **Data Modeling & BI:** Power BI (Star Schema, DAX)
* **Version Control:** Git & GitHub

---

## 📊 Power BI Dashboards
The Gold layer feeds directly into a multi-page interactive Power BI report tailored for stakeholders:
* **Executive Dashboard:** Tracks overall Total Revenue, Conversion Rates, Units Sold, Cancellation Rates, and performance by brokers and payment methods.
* **Marketing Dashboard:** Analyzes marketing costs, ROAS, Cost Per Lead (CPL), Cost Per Click (CPC), and campaign-level performance across channels.
* **Customers Dashboard:** Evaluates buyer distributions by city, lead sources, and acquisition efficiency.

---

## 👨‍💻 Author
**Bassem Elgwaily**
