# NYC Payroll Data Pipeline Project

## 📌 Project Overview
This project implements a complete **data engineering pipeline** for processing and analyzing **NYC Payroll data** using **Azure Data Factory, Azure Data Lake, SQL Database, and Synapse Analytics**.

The pipeline automates the ingestion, transformation, and aggregation of payroll data to support analytical insights.

---

## ⚙️ Tech Stack & Tools
- **Azure Data Lake Storage (ADLS)** – Raw and processed data storage
- **Azure Data Factory (ADF)** – Data ingestion, transformation, and orchestration
- **Azure SQL Database** – Transactional data storage
- **Azure Synapse Analytics** – Data aggregation and analytics using external tables

---

## 🚀 Project Workflow

### Step 1: Prepare the Data Infrastructure
- Created Data Lake containers and directories:
  - `Dirpayrollfiles` (for payroll datasets)
  - `Dirhistoryfiles` (for historical files)
- Provisioned:
  - Azure Data Factory
  - SQL Database
  - Synapse Analytics Workspace

### Step 2: Create Linked Services
- Configured connections between ADF, ADLS, SQL DB, and Synapse.

### Step 3: Create Datasets in ADF
- Defined datasets for payroll and historical files.

### Step 4: Build Data Flows
- Developed **data transformation flows** to clean and load payroll data into SQL DB.

### Step 5: Data Aggregation & Parameterization
- Implemented parameterized dataflows for flexible ingestion by fiscal year.
- Aggregated payroll data for reporting and analytics.

### Step 6: Pipeline Creation
- Designed and executed end-to-end pipeline in **ADF**.
- Verified successful runs without errors.

---

## 📊 Outputs
- **SQL DB**: Master data tables and payroll transaction tables.
- **Synapse Analytics**: External summary tables for quick analytical queries.
- **Data Lake**: Organized staging and processed datasets.

---

## 📷 Screenshots (Available in Report)
- Data Lake staging directory listing
- Synapse summary external tables
- SQL DB query outputs

---

## 📈 Key Learnings
- Orchestration with **ADF pipelines**
- Data storage best practices with **ADLS & SQL DB**
- Scalable analytics using **Synapse external tables**
- Parameterized workflows for reusability

---

## 📝 How to Run This Project
1. Provision Azure resources: ADLS, ADF, SQL DB, and Synapse.
2. Upload payroll files into the Data Lake (`Dirpayrollfiles`).
3. Configure linked services in ADF.
4. Deploy datasets and dataflows.
5. Execute the pipeline and verify the outputs in SQL DB & Synapse.

---

## 📚 References
- [Azure Data Factory Documentation](https://learn.microsoft.com/en-us/azure/data-factory/)
- [Azure Synapse Analytics Documentation](https://learn.microsoft.com/en-us/azure/synapse-analytics/)
"""
