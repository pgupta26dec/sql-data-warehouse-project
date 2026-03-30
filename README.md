# 📊 SQL Data Warehouse & Analytics Project

A comprehensive, end-to-end data warehousing and analytics solution that demonstrates modern data engineering practices. This project transforms raw data from ERP and CRM systems into actionable business insights using **SQL Server**, the **Medallion Architecture**, and **Star Schema** modeling.

---

## 🏗️ Data Architecture: The Medallion Approach
The project follows the **Medallion Architecture** to ensure data quality and separation of concerns across three distinct layers:

* **🟫 Bronze Layer (Raw):** Ingests raw data "as-is" from CSV source files (ERP & CRM) into SQL Server. The focus here is on data traceability and integrity.
* **⬜ Silver Layer (Cleaned):** Implements data cleansing, normalization, and standardization. This layer resolves issues like duplicates, null values, and inconsistent formatting to prepare the data for business logic.
* **🟨 Gold Layer (Business):** The final layer containing "business-ready" data. It is modeled using a **Star Schema** with Fact and Dimension tables, optimized for high-performance analytical queries and reporting.



---

## 🛠️ Tech Stack & Tools
* **Database Engine:** SQL Server Express
* **Environment:** SQL Server Management Studio (SSMS)
* **Data Modeling:** Star Schema (Fact & Dimension tables)
* **Workflow Design:** Draw.io (Architecture diagrams)
* **Language:** T-SQL (Stored Procedures, DDL, DML)

---

## 📂 Project Structure
```text
sql-data-warehouse-project/
├── datasets/             # Raw ERP and CRM CSV files
├── scripts/              # SQL scripts for ETL and Database setup
│   ├── init_database.sql # Database and schema initialization
│   ├── bronze/           # DDL and Bulk Insert scripts for Bronze layer
│   ├── silver/           # Cleansing and transformation scripts for Silver layer
│   └── gold/             # Views and Star Schema logic for Gold layer
├── tests/                # Data quality and integrity checks
└── docs/                 # Architecture visuals and data model documentation
