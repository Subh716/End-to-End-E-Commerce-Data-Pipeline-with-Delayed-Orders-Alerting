# End-to-End-E-Commerce-Data-Pipeline-with-Delayed-Orders-Alerting
End-to-end e-commerce data pipeline with Snowflake, dbt &amp; Airflow — featuring alerting for delayed orders and modular ELT workflows.
This project demonstrates a full-stack data engineering pipeline for a simulated e-commerce platform using **Snowflake**, **dbt**, and **Apache Airflow**. It covers ingestion, transformation, orchestration, and monitoring — with a built-in alerting system for delayed orders.


## Project Overview

This pipeline simulates order data flowing through a cloud-native data stack, transforming raw records into actionable insights. It includes:

- ELT pipeline processing ~3 Million order records
- Modular medallion architecture in Snowflake (Bronze → Silver → Gold)
- Data modeling with dbt (fact and dimension tables)
- Scheduled ELT workflows with Apache Airflow DAGs
- Email alerts triggered for orders delayed beyond expected delivery time


## Tech Stack

- **Cloud Data Warehouse:** Snowflake
- **Transformation Layer:** dbt
- **Workflow Orchestration:** Apache Airflow
- **Programming Languages:** SQL, Python
- **Other Tools:** Git, Jinja, Email Alerting


## Features

- Simulates e-commerce order lifecycle and delay tracking
- Builds fact/dim models with dbt for clean, tested analytics-ready data
- Schedules workflows with Airflow, including automated retries
- Sends email alerts for 200+ delayed orders based on defined business logic
- Supports downstream reporting and BI use cases


## Architecture Diagram

> *(Optional: Insert a diagram.png or use draw.io to visualize the medallion architecture + Airflow orchestration)*



## Folder Structure

```
ecommerce-data-pipeline/
├── airflow/               # DAGs for scheduling & alerts
├── dbt_project/           # dbt models (staging, marts)
├── data/                  # Sample data files
├── docs/                  # Pipeline architecture diagram
├── requirements.txt       # Project dependencies
└── README.md              # Project overview and instructions
```
