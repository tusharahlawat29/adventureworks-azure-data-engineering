
# 🚀 AdventureWorks Azure Data Engineering Project

![Azure](https://img.shields.io/badge/Azure-Data%20Engineering-blue)
![ADF](https://img.shields.io/badge/Azure%20Data%20Factory-Ingestion-orange)
![Databricks](https://img.shields.io/badge/Databricks-Spark-red)
![Synapse](https://img.shields.io/badge/Synapse-Analytics-blue)
![Python](https://img.shields.io/badge/Python-SparkSQL-yellow)

---

## 📌 Project Overview

A fully end-to-end **data engineering pipeline** built on **Microsoft Azure**, designed to showcase real-world skills in **data ingestion, transformation, storage optimization, and analytics**.
This project replicates a modern data engineering workflow using **enterprise-grade tools**:

* Azure Data Factory (ADF)
* Azure Data Lake Storage Gen2 (ADLS)
* Azure Databricks (Spark)
* Azure Synapse Analytics

The pipeline follows a **Medallion Architecture (Bronze → Silver → Gold)** for structured data processing.

---

## 🏗️ Architecture

```
On-Prem Source → Azure Data Factory → ADLS (Bronze → Silver → Gold)
                                              ↓
                                      Azure Databricks
                                              ↓
                                      Azure Synapse Analytics
```

**Architecture Diagram:** `architecture/project-diagram.png` 
<img width="901" height="689" alt="project-diagram" src="https://github.com/user-attachments/assets/c92e8922-d79b-49f1-8de6-6a439b335450" />


---

## 🛠️ Technologies Used

| Layer          | Service / Tool               |
| -------------- | ---------------------------- |
| Data Ingestion | Azure Data Factory           |
| Storage        | Azure Data Lake Storage Gen2 |
| Transformation | Azure Databricks (Spark)     |
| Data Model     | Delta Lake                   |
| Analytics      | Azure Synapse Analytics      |
| Programming    | Python, Spark SQL            |

---

## 📂 Project Structure

```
adventureworks-azure-data-engineering/
│
├── data/                         # Sample CSV files (small size only)
│
├── architecture/
│   └── project-diagram.png       # Architecture diagram
│
├── notebooks/
│   └── databricks_notebooks.py   # Spark transformation code
│
├── adf/
│   └── pipeline.json             # Azure Data Factory pipeline
│
├── sql/
│   └── synapse_queries.sql       # Synapse SQL queries
│
├── screenshots/                  # Screenshots of pipelines / outputs
│
└── README.md                     # Project documentation
```

---

## 🚀 Pipeline Steps

### 1️⃣ Data Ingestion — Azure Data Factory

* Created **linked services** for ADLS and source storage
* Built a **dynamic pipeline** using JSON metadata
* Ingested raw CSV files into **Bronze layer** of ADLS

### 2️⃣ Data Transformation — Azure Databricks

* Mounted ADLS to Databricks workspace
* Read Bronze layer files using Spark
* Performed **data cleaning, validation, deduplication, schema enforcement**
* Wrote optimized **Delta tables** to Silver and Gold layers

### 3️⃣ Data Analytics — Azure Synapse

* Connected Synapse to ADLS Gold layer
* Created **external tables** and **views**
* Performed analytical queries for business insights
* Verified **data quality** and reporting readiness

---

## 📊 Output / Deliverables

* Cleaned and transformed **Delta tables** in Gold layer
* Business-ready analytics insights from Synapse
* End-to-end reusable Azure data pipeline

---

## 📘 Key Learning Outcomes

✔ Azure cloud data engineering best practices
✔ Dynamic pipelines in Azure Data Factory
✔ Spark transformations in Databricks (Bronze → Silver → Gold)
✔ Data Lake architecture & Delta Lake optimization
✔ End-to-end integration with Synapse Analytics
✔ Analytical insights generation and Power BI integration

---


## 💼 Resume / Project Summary

**Azure Data Engineering Project — AdventureWorks Dataset**
Built a **complete Azure-based data pipeline** using ADF, ADLS Gen2, Databricks, and Synapse.
Designed ingestion workflows, implemented Spark-based transformations (Bronze → Silver → Gold model), optimized Delta Lake tables, and enabled analytical reporting using Synapse SQL.

---

## 📣 Author

**Tushar Ahlawat**
Aspiring Data Engineer | Azure & Databricks Enthusiast

