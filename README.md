**1. Overview**

**This repository showcases an end-to-end Data Engineering pipeline using the NYC Taxi dataset on Microsoft Azure.**
**It demonstrates how to ingest, process, and deliver business-ready data for analytics using:**
**ADLS Gen2, ADF, Azure Databricks, Delta Lake, and Power BI.**
**The project follows the Medallion Architecture (Bronze 🥉, Silver 🥈, Gold 🥇) to ensure scalability, reliability, and high data quality.**


**2. Architecture 🏗️**

**Data Flow:**

**Source Data: NYC Taxi Trip Data (Green/Yellow/For-Hire).**

**Bronze Layer 🥉: Raw ingestion in ADLS Gen2 with metadata.**

**Silver Layer 🥈: Cleansing, schema enforcement, deduplication, & validation in Delta Lake.**

**Gold Layer 🥇: Aggregated KPIs (Revenue 💰, Trips 🚕, Geo Insights 🌍).**

**Orchestration 🔄: ADF triggers Databricks notebooks for ETL.**

**Consumption 📊: Power BI dashboards via Databricks SQL Endpoint.**

**Tech Stack 🛠️**

-**Azure Data Lake Storage Gen2 🗂️**

-**Azure Data Factory 🔄**

-**Azure Databricks (PySpark, Delta Lake) ⚡**

-**Azure Key Vault 🔐**

-**Power BI 📊**

**1. Data Outputs (Delta Tables in ADLS)**

**Bronze Layer (Raw):**

**Ingested NYC Taxi trip data in original format with metadata (ingestion timestamp, source file info).**

**Silver Layer (Cleaned & Validated):**

**Standardized schema, deduplicated trips, filtered invalid fares/distances.**

**Gold Layer (Curated):**

**Daily KPIs (Revenue, Trips, Avg Distance), Monthly trends, Top pickup/drop-off zones.**
