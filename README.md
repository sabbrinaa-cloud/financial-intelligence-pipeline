# 💼 Financial Intelligence Pipeline

### End-to-End Financial Intelligence Solution using SQL Server, Power BI, n8n and Dimensional Modeling

---

## 📌 Overview

The **Financial Intelligence Pipeline** is an end-to-end Business Intelligence project designed to automate the ingestion, transformation, modeling and visualization of financial data.

The solution combines **SQL Server**, **Stored Procedures**, **n8n**, **Power BI** and **Dimensional Modeling** to build a reliable analytical environment capable of supporting executive decision-making.

---

## 🎯 Project Objectives

- Automate the ETL process
- Standardize financial data
- Build a dimensional model
- Deliver executive dashboards
- Provide operational analysis
- Centralize business rules in SQL Server
- Automate execution using n8n

---

## 🛠 Technologies

| Technology | Purpose |
|------------|---------|
| SQL Server 2022 | Relational database and ETL processing |
| T-SQL Stored Procedures | Business rules, transactional processing and data loading |
| n8n | ETL workflow orchestration and scheduling |
| Power BI Desktop | Executive and analytical dashboards |
| DAX | KPIs, Time Intelligence and Smart Tooltips |
| Dimensional Modeling | Star Schema (Facts & Dimensions) |
| CSV Files | Source data |
| Git & GitHub | Version control and project documentation |

---

## 🏗️ Solution Architecture

The following diagram illustrates the complete architecture of the Financial Intelligence Pipeline.

The solution starts with CSV source files, loads the data into SQL Server through reusable Stored Procedures, orchestrates the ETL with n8n, applies dimensional modeling, and finally delivers executive analytics in Power BI.

<p align="center">
    <img src="Docs/Slides/01_Arquitetura_Geral.png" width="900">
</p>

---

## 🔄 ETL Pipeline

The ETL process is fully orchestrated using reusable SQL Server Stored Procedures and automated through n8n.

The pipeline follows a modular architecture where each entity is imported, validated and processed independently before being loaded into the dimensional model.

### Main processing flow

1. Import CSV files into staging tables.
2. Validate data integrity and business rules.
3. Process entities through dedicated Stored Procedures.
4. Execute the complete transactional workflow.
5. Load data into dimensional tables.
6. Make the data available for Power BI dashboards.

<p align="center">
    <img src="Docs/Slides/06_Pipeline_ETL.png" width="950" alt="ETL Pipeline">
</p>

---

## ⚙️ Workflow Automation (n8n)

The execution of the ETL pipeline is fully automated using n8n.

The workflow is responsible for scheduling the execution, triggering SQL Server Stored Procedures and monitoring the execution status, reducing manual intervention and ensuring process consistency.

<p align="center">
    <img src="Docs/Slides/07_Workflow_n8n.png" width="900" alt="n8n Workflow">
</p>

<p align="center">
    <img src="Docs/Slides/08_Execucao_orquestrada_n8n.png" width="900" alt="Workflow Execution">
</p>

---

## 🗄️ Dimensional Data Model

The Financial Intelligence Pipeline uses a Star Schema dimensional model to optimize analytical queries and Power BI performance.

The model separates transactional data into Facts and Dimensions, providing scalability, consistency and high-performance reporting.

### Main Components

- Fact Tables
- Dimension Tables
- Business Keys
- Surrogate Keys
- Referential Integrity
- Optimized relationships for analytics

<p align="center">
    <img src="Docs/Slides/05_Modelo_Dados_SQL.png" width="900" alt="Dimensional Data Model">
</p>


