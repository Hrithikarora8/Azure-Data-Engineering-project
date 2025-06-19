# 🚀 End-to-End Data Engineering Pipeline with Medallion Architecture on Azure

**🗂 Dataset:** AdventureWorks  
**🕒 Duration:** Jan 2025 – Feb 2025  
**👨‍💻 Role:** Data Engineer  
**🛠 Tools & Technologies:**  
Azure Data Factory | Azure Data Lake Storage Gen2 | Azure Databricks (PySpark) | Azure Synapse Analytics | Power BI | SQL | Delta Lake

---

## 📚 Project Overview

Designed and implemented a complete data engineering pipeline using Microsoft Azure services to demonstrate a scalable data ingestion-to-reporting lifecycle using the **AdventureWorks** dataset. This solution follows the **Medallion Architecture** — Bronze, Silver, and Gold layers — to separate raw, refined, and business-level data processing.

---

## 🏗️ Data Architecture

```text
GitHub CSV (AdventureWorks)
        |
[ADF] → Bronze Layer (Raw)
        |
[Databricks (PySpark)] → Silver Layer (Cleaned & Structured)
        |
[Views + External Tables]
        ↓
Gold Layer (Aggregated Business Data)
        ↓
[Synapse SQL Pool] → [Power BI]
