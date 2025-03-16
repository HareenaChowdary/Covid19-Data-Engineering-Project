
# COVID-19 Data Engineering Project

## Overview
This project focuses on building a data platform for reporting and predicting the spread of COVID-19. The goal is to ingest, process, and store COVID-19-related data, enabling data analysts to generate reports and data scientists to apply machine learning models for insights.

## Objectives
1. **Data Platform for ML Models**: Provide a structured data lake for running machine learning models to predict virus spread.
2. **Reporting Platform**: Enable data analysts to generate reports on COVID-19 trends using Power BI.

## Data Sources
- **European Centre for Disease Prevention and Control (ECDC)**: Confirmed cases, mortality, hospitalization, ICU cases, and testing data.
- **Eurostat**: Population data by age group.

## Solution Architecture
1. **Data Ingestion**:
   - **COVID-19 Data**: Retrieved using the HTTP connector in Azure Data Factory.
   - **Population Data**: Stored in Azure Blob Storage and ingested via Azure Data Factory.
2. **Data Storage**:
   - **Azure Blob Storage**: Stores raw population data.
   - **Azure Data Lake Storage Gen2**: Main data lake for processing and storage.
   - **Azure SQL Database**: Data warehouse for structured reporting.
3. **Data Transformation**:
   - **Azure Data Factory Data Flows**: Code-free transformations for simpler processing.
   - **Azure HDInsight & Databricks**: Used for scalable, distributed data transformations.
4. **Orchestration**:
   - Azure Data Factory orchestrates all data processing workflows.
5. **Reporting**:
   - Power BI dashboards created using processed data from Azure SQL Database.

## Technologies Used
- **Azure Services**: Data Factory, Blob Storage, Data Lake Storage Gen2, SQL Database, HDInsight, Databricks
- **Data Processing**: PySpark, Spark SQL, Hive
- **Visualization**: Power BI

## 🚀 Setup Instructions

### 1️⃣ Prerequisites
Ensure you have the following:
- An **Azure subscription**.
- **Azure Data Factory, Blob Storage, Azure Data Lake Storage Gen2, and Azure SQL Database** set up.
- Power BI installed for reporting.

### 2️⃣ Data Ingestion
- Configure **Azure Data Factory** to pull COVID-19 data from the **ECDC API**.
- Store **Population Data** in **Azure Blob Storage** and set up ADF ingestion.

### 3️⃣ Data Transformation
- Use **Azure Data Factory Data Flows** to clean and structure the data.
- Implement additional transformations in **Azure Databricks and HDInsight**.

### 4️⃣ Data Storage
- Store processed data in **Azure Data Lake Storage Gen2**.
- Load necessary data into **Azure SQL Database** for reporting.

### 5️⃣ Data Visualization
- Connect Power BI to **Azure SQL Database** to create reports.

## 📊 Power BI Reporting
- Visualize **COVID-19 trends**: cases, hospitalizations, mortality rates, and testing numbers.
- Reports include **weekly trends, age-wise statistics, and country-level comparisons**.






