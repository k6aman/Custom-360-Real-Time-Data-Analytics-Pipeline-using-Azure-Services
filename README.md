# Custom 360 – Real-Time Data Analytics Pipeline using Azure Services
# 📌 Project Overview

Custom 360 is an end-to-end data analytics pipeline built on Microsoft Azure to integrate, process, and analyze data from multiple sources using the Medallion Architecture (Bronze–Silver–Gold). The project automates data ingestion from APIs and on-premise systems, performs scalable transformations using Spark, and delivers analytics-ready data to empower business reporting in Power BI.


## 🛠️ Architecture Diagram

```mermaid
flowchart TD
    A["Data Source (API / On-Premise)"] --> B["Azure Data Factory (Ingestion & Orchestration)"]
    B --> C["Bronze Layer - Azure Data Lake Storage (Raw Data)"]
    C --> D["Silver Layer - Azure Databricks (PySpark Transformations)"]
    D --> E["Gold Layer - Azure SQL Database (Curated Data)"]
    E --> F["Power BI (Analytics & Dashboard)"]


# 📂 Data Flow

1. Extract data from HTTP REST APIs and on-premise systems.
2. Load raw data into Bronze layer (ADLS).
3. Transform and clean data in Silver layer using Spark.
4. Apply business logic & optimization.
5. Load curated tables into Gold layer (Azure SQL DB).
6. Connect dataset to Power BI for dashboarding.
