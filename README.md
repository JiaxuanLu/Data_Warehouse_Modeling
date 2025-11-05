## Project Overview  

This project builds a modern **data warehouse** for the classic **Northwind** dataset, integrating sales, purchasing, and inventory data to enable advanced analytics and BI reporting.  
The pipeline follows a **modular ELT architecture** using **dbt** for transformation, with **PostgreSQL** as the source system and **Snowflake** as the target cloud data warehouse.  


## Objectives  

- Centralize and standardize data from multiple Northwind operational sources.  
- Implement a **three-layer dbt modeling structure**: *staging*, *warehouse*, and *analytics OBT (One Big Table)*.  
- Create **dimensional models (star schema)** for customer, product, employee, and order analysis.  
- Provide **analytics-ready datasets** to support reporting in BI tools such as Power BI or Looker.  


## Project Architecture  
northwind-data-warehouse/
│
├── models/
│   ├── northwind/
│   │   ├── staging/               # Data cleaning and standardization
│   │   ├── warehouse/             # Fact and dimension tables
│   │   └── analytics_obt/         # Business-ready reporting tables
│   │
│   └── practice_project_jaffle_shop/  # Reference dbt project for testing
│
├── seeds/                         # Static reference datasets
├── tests/                         # Custom and generic dbt tests
├── macros/                        # Reusable SQL macros
├── snapshots/                     # Historical tracking (future expansion)
├── analyses/                      # Exploratory SQL analyses
└── dbt_project.yml

