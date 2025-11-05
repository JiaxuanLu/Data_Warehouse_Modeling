# Northwind Data Warehouse

A modern **data warehouse project** built with **dbt** on **Snowflake**, using the classic **Northwind** sales dataset.  
This project demonstrates how to design a scalable ELT pipeline with clear modeling layers — from raw data to business-ready analytics tables.


## Project Overview

The goal of this project is to transform the Northwind sales database into a **dimensional data warehouse** that supports sales, inventory, and purchasing analytics.


### Project Architecture

| Path | Purpose |
|---|---|
| `northwind-data-warehouse/` | Repository root |
| `models/` | dbt models root |
| `models/northwind/` | Northwind project models |
| `models/northwind/staging/` | Data cleaning and standardization |
| `models/northwind/warehouse/` | Fact and dimension tables |
| `models/northwind/analytics_obt/` | Business-ready reporting tables |
| `models/practice_project_jaffle_shop/` | Reference dbt project for testing |
| `seeds/` | Static reference datasets |
| `tests/` | Custom and generic dbt tests |
| `macros/` | Reusable SQL macros |
| `snapshots/` | Historical tracking (future expansion) |
| `analyses/` | Exploratory SQL analyses |
| `dbt_project.yml` | dbt project config |
