# Custom 360 – Real-Time Data Analytics Pipeline using Azure Services
# 📌 Project Overview

Custom 360 is an end-to-end data analytics pipeline built on Microsoft Azure to integrate, process, and analyze data from multiple sources using the Medallion Architecture (Bronze–Silver–Gold). The project automates data ingestion from APIs and on-premise systems, performs scalable transformations using Spark, and delivers analytics-ready data to empower business reporting in Power BI.

# 🛠️ Architecture Diagram

Data Source (API/On-Prem) 
        │
        ▼
 Azure Data Factory (Ingestion & Orchestration)
        │
        ▼
 Bronze Layer – Azure Data Lake Storage (Raw Data)
        │
        ▼
 Silver Layer – Azure Databricks (Transformations using PySpark)
        │
        ▼
 Gold Layer – Azure SQL Database (Serving Layer)
        │
        ▼
 Power BI (Analytics & Dashboard)


# 📂 Data Flow

1. Extract data from HTTP REST APIs and on-premise systems.
2. Load raw data into Bronze layer (ADLS).
3. Transform and clean data in Silver layer using Spark.
4. Apply business logic & optimization.
5. Load curated tables into Gold layer (Azure SQL DB).
6. Connect dataset to Power BI for dashboarding.
