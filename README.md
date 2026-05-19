# Azure-end-to-end-data-engineer-project

## Overview
This project demonstrates an end-to-end Azure Data Engineering pipeline using Azure Data Factory (ADF), Azure Data Lake Storage (ADLS), Databricks, Delta Lake, and Power BI. It follows the Medallion Architecture (Bronze → Silver → Gold) to build a scalable and efficient data processing solution for retail sales analytics.

## Tech Stack
Azure Data Factory (ADF)
Azure Data Lake Storage (ADLS) / Azure Blob Storage
Azure Databricks
Delta Lake
Power BI

## Data Pipeline Workflow
### Data Ingestion

Ingested data from multiple sources:

API-based JSON data (GitHub)
Raw Parquet files (Retail datasets)

Built and published ETL pipelines in Azure Data Factory
Loaded data into Azure Data Lake Storage (Bronze Layer)

## Bronze Layer (Raw Data)

Stored raw data as-is in ADLS
Maintained source-level datasets for:

Transactions
Products
Stores
Customers

## Silver Layer (Cleaned & Transformed Data)

Processed data using Azure Databricks
Applied transformations:

Data type conversions
Duplicate removal
Data quality improvements


Created structured Delta tables for each entity


## Gold Layer (Business-Level Aggregation)

Combined datasets for analytics
Built aggregated tables with key metrics:

Total Sales
Quantity Sold
Transaction Count
Average Transaction Value


## Data Validation

Performed validation using:

Spark SQL
DataFrame checks


Ensured data accuracy at each stage


## Power BI Dashboard

Built an interactive Retail Sales Dashboard
Key KPIs:

Total Sales: 134.57K
Total Quantity Sold: 101
Total Transactions: 30


## Visualizations:

Monthly Sales Trend (Line Chart)
Product-wise Sales Distribution (Pie Chart)


Focused on clean layout, formatting, and insights


## Key Achievements

Implemented a complete Medallion Architecture pipeline
Integrated multiple data sources into a unified system
Built scalable Delta Lake storage model
Delivered actionable insights via Power BI


## Future Enhancements

Advanced DAX calculations for deeper insights
Real-time data processing
Performance optimization and scheduling improvements
