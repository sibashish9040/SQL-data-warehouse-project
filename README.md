# SQL-data-warehouse-project
Welcome to the Data Warehouse and Analytics Project repository! 🚀
This project demonstrates a comprehensive data warehousing and analytics solution, from building a data warehouse to generating actionable insights. Designed as a portfolio project, it highlights industry best practices in data engineering and analytics.

If you want to follow up with my project you can checkout my notion file with detailed procedure and techniques below:

<img width="30" height="30" src="https://img.icons8.com/ios/50/FFFFFF/notion.png" alt="notion"/>[Notion](https://elated-november-3de.notion.site/Data-Warehouse-Project-22b421886a4080dead78c2e5d98804ab?source=copy_link)

-----------------------------------------------------------
# 🏗️ Data Architecture
The data architecture for this project follows Medallion Architecture Bronze, Silver, and Gold layers:
![data architecture diagram](https://github.com/sibashish9040/SQL-data-warehouse-project/blob/main/docs/Data%20architecture%20diagram.drawio.png)
1. Bronze Layer: Stores raw data as-is from the source systems. Data is ingested from CSV Files into SQL Server Database.
2. Silver Layer: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
3. Gold Layer: Houses business-ready data modeled into a star schema required for reporting and analytics.
------
# 📖 Project Overview
This project involves:

- Data Architecture: Designing a Modern Data Warehouse Using Medallion Architecture Bronze, Silver, and Gold layers.
- ETL Pipelines: Extracting, transforming, and loading data from source systems into the warehouse.
- Data Modeling: Developing fact and dimension tables optimized for analytical queries.
- Analytics & Reporting: Creating SQL-based reports and dashboards for actionable insights.

🎯 This repository showcase my following skills:

- SQL Development
- Data Architect
- Data Engineering
- ETL Pipeline Developer
- Data Modeling
- Data Analytics

# 📂 Repository Structure
```
data-warehouse-project/
│
├── datasets/                           # Raw datasets used for the project (ERP and CRM data)
|   ├── source_crm                      # contains raw data set from crm source    
|   ├── source_erp                      # contains raw data set from erp source
│
├── docs/                               # Project documentation and architecture details
│   ├── etl.drawio                      # Draw.io file shows all different techniquies and methods of ETL
│   ├── Data architecture
|       diagram.drawio.png              # Draw.io file shows the project's architecture
│   ├── data_catalog.md                 # Catalog of datasets, including field descriptions and metadata
│   ├── data_flow.drawio                # Draw.io file for the data flow diagram
│   ├── data_models.drawio              # Draw.io file for data models (star schema)
│   ├── naming-conventions.md           # Consistent naming guidelines for tables, columns, and files
│
├── scripts/                            # SQL scripts for ETL and transformations
│   ├── bronze/                         # Scripts for extracting and loading raw data
│   ├── silver/                         # Scripts for cleaning and transforming data
│   ├── gold/                           # Scripts for creating analytical models
│
├── tests/                              # Test scripts and quality files
│
├── README.md                           # Project overview and instructions
├── LICENSE                             # License information for the repository
├── .gitignore                          # Files and directories to be ignored by Git
└── requirements.txt                    # Dependencies and requirements for the project
```
-----
# 🛠️ Tools & Technologies

- **SQL Server** – Data warehousing and analytics engine
- **Draw.io** – Architecture and modeling diagrams
- **SSMS(SQL SERVER MANAGEMENT STUDIO version 2022)** – Development environment
- **Notion** – Documentation
- **Git** – Version control

# 🚀 Getting Started

Follow these steps to set up and run the project locally:

### 1. Clone the Repository

```bash
git clone https://github.com/sibashish9040/SQL-data-warehouse-project.git
cd SQL-data-warehouse-project
```
- Install and configure a SQL Server instance.
- Use any SQL client, I have used SQL Server Management Studio (SSMS) to run SQL scripts.
```
# Bronze Layer
#run the ddl_bronze.sql file first, then modify the load_bronze file according to your file location
#run the load_bronze.sql file
scripts/bronze/*.sql

# Silver Layer
# run the ddl_silver.sql and then load_silver.sql
scripts/silver/*.sql

# Gold Layer
# run the gold_views.sql for the final view creation 
scripts/gold/*.sql
```

----

# 📄 License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.

