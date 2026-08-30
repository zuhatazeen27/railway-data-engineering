# 🚆 Railway Data Engineering Pipeline

An end-to-end data engineering project built using **Databricks, PySpark, SQL, Delta Lake, and GitHub** to process, transform, validate, and analyze railway service data.

The project follows the **Medallion Architecture (Bronze → Silver → Gold)** and includes data ingestion, data transformation, analytical aggregations, data-quality auditing, and an interactive Databricks dashboard.

## 📌 Project Overview

This project builds a complete data engineering pipeline for railway service data.

Raw railway data is ingested into the **Bronze layer**, cleaned and transformed in the **Silver layer**, and then aggregated into business-ready datasets in the **Gold layer**.

A dedicated **Data Quality Audit** process validates the pipeline and tracks record counts and pipeline status.

The final Gold-layer data is used to create an interactive **Railway Data Engineering Dashboard** in Databricks.

## 🏗️ Architecture

                   RAW RAILWAY CSV
                          │
                          ▼
                ┌───────────────────┐
                │   BRONZE LAYER    │
                │ Raw Data Ingestion │
                └─────────┬─────────┘
                          │
                          ▼
                ┌───────────────────┐
                │   SILVER LAYER    │
                │ Cleaning &        │
                │ Transformation    │
                └─────────┬─────────┘
                          │
                          ▼
                ┌───────────────────┐
                │    GOLD LAYER     │
                │ Aggregation &     │
                │ Analytics         │
                └─────────┬─────────┘
                          │
              ┌───────────┴───────────┐
              ▼                       ▼
       Data Quality Audit      Databricks Dashboard


## 📂 Project Structure
railway-data-engineering/
│
├── 01_Bronze_Railway_Ingestion.ipynb
├── 02_Silver_Railway_Transformation.ipynb
├── 03_Gold_Railway_Aggregation.ipynb
├── 04_Data_Quality_Audit.ipynb
└── README.md

## 🥉 Bronze Layer

The Bronze layer ingests raw railway data into Databricks.

### Operations

- Read raw CSV data using PySpark
- Preserve source data
- Create Bronze Delta table
- Store raw railway records
- Track ingestion information

## 🥈 Silver Layer

The Silver layer cleans and transforms the Bronze data.

### Operations

- Data cleaning
- Data type conversion
- Handling missing values
- Standardizing values
- Creating derived columns
- Removing invalid records
- Creating a cleaned railway dataset

## 🥇 Gold Layer

The Gold layer contains business-ready analytical datasets.

### Analysis Includes

- Train services by source station
- Train services by destination station
- Train services by route
- Day-wise train distribution
- Weekday vs weekend train activity

## 📊 Databricks Dashboard

An interactive dashboard was created in Databricks to analyze railway service activity.

### Dashboard Components

- 🚆 Total Train Services
- 🚉 Top 10 Source Stations
- 📅 Day-wise Train Distribution
- 📊 Weekday vs Weekend Services
- 🛤️ Top Train Routes
- 🚉 Source → Destination Service Analysis

### Key Metric

**Total Train Services: 11,113**

## 🛡️ Data Quality Audit

A dedicated audit notebook validates the pipeline and tracks data-processing metrics.

### Audit Metrics

- Bronze record count
- Silver record count
- Gold station records
- Gold route records
- Gold day records
- Gold day-type records
- Pipeline status
- Audit timestamp

The audit helps verify that data is successfully processed through the Bronze, Silver, and Gold layers.

## 🧰 Technologies Used

| Technology | Purpose |
|---|---|
| Python | Data engineering development |
| PySpark | Distributed data processing |
| SQL | Data analysis |
| Databricks | Data engineering platform |
| Delta Lake | Data storage |
| Git | Version control |
| GitHub | Source code management |
| Databricks Dashboard | Data visualization |

## 🧠 Skills Demonstrated

- ETL / ELT Pipeline Development
- Medallion Architecture
- PySpark
- SQL
- Data Ingestion
- Data Cleaning
- Data Transformation
- Data Aggregation
- Delta Lake
- Data Quality Validation
- Data Auditing
- Data Analytics
- Dashboard Development
- Git & GitHub

## 🔄 End-to-End Workflow

Raw Railway CSV
      ↓
Bronze Data Ingestion
      ↓
Bronze Delta Table
      ↓
Data Cleaning & Transformation
      ↓
Silver Cleaned Table
      ↓
Gold Aggregations
      ↓
Data Quality Audit
      ↓
Databricks Dashboard
      ↓
Business Insights

## 📈 Project Results

The pipeline successfully processes railway service data through the Bronze, Silver, and Gold layers and produces business-ready analytical datasets.

### Key Results

| Metric | Result |
|---|---:|
| Total Records | 11,113 |
| Unique Trains | 11,113 |
| Unique Source Stations | 921 |
| Unique Destination Stations | 924 |
| Top Source Station | CST-MUMBAI |
| Top Source Services | 513 |
| Top Destination Station | CST-MUMBAI |
| Top Destination Services | 514 |
| Weekday Services | 7,918 |
| Weekend Services | 3,195 |
| Most Frequent Route | TAMBARAM → CHENNAI BEACH |
| Top Route Services | 137 |

## 💡 Key Insights

- 🚉 CST-MUMBAI is one of the major railway hubs in the analyzed dataset.
- 🛤️ TAMBARAM → CHENNAI BEACH is the most frequent route identified.
- 📅 Weekday services are significantly higher than weekend services.
- 🚆 The dataset contains more than 11K railway service records.
- 📊 Day-wise analysis reveals differences in train activity throughout the week.
- 🔍 Station and route-level aggregation provides useful operational insights.

## 🎯 Resume Project Description

**Railway Data Engineering Pipeline | Databricks, PySpark, SQL, Delta Lake**

Developed an end-to-end railway data engineering pipeline using Databricks and PySpark following Medallion Architecture. Implemented Bronze data ingestion, 
Silver data transformation, Gold analytical aggregations, data-quality auditing, and an interactive Databricks dashboard to analyze 11K+ railway service records across stations, routes, and operating days.

## 🚀 Future Improvements

- Incremental data processing
- Advanced data-quality checks
- Pipeline failure alerts
- Real-time railway data ingestion
- Historical trend analysis
- Parameterized dashboards
- Automated testing
- CI/CD integration
- Cloud-based production deployment

## 👩‍💻 Author

**Zuha Tazeen**

GitHub: [@zuhatazeen27](https://github.com/zuhatazeen27)

## ⭐ Project Highlights

- ✓ End-to-end Data Engineering Pipeline
- ✓ Medallion Architecture
- ✓ Bronze → Silver → Gold
- ✓ PySpark
- ✓ SQL
- ✓ Delta Lake
- ✓ Data Quality Audit
- ✓ Databricks Job
- ✓ Databricks Dashboard
- ✓ Git & GitHub
- ✓ 11K+ Railway Records Analyzed
