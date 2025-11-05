# Data Engineering Assignment 10 – Airflow ETL Pipeline
Data Engineering Assignment 10


# 📌 Project Overview

This project demonstrates deploying Apache Airflow in a development environment and creating an automated ETL pipeline. The pipeline ingests data from multiple sources, performs transformations, merges the datasets, and loads the processed data into a PostgreSQL database. Finally, analytical tasks are performed on the transformed data, including visualization and cleanup of intermediate data.


## 📁 Directory Structure
DATA-ENGINEERING-ASSIGNMENT10/
│
├── .devcontainer/ # Development container config
├── airflow-env/ # Python virtual environment for Airflow
│
├── dags/
│ ├── pipeline.py # Main DAG implementation
│ └── __pycache__/
│
├── data/ # Raw and processed datasets
├── logs/ # Airflow logs
├── pics/ # Visualization output (e.g., Pipeline.png)
├── plugins/ # Custom Airflow plugins (if any)
│
├── airflow.cfg # Airflow configuration
├── requirements.txt # Python dependencies
└── README.md


DAG Graph

Output screenshot saved as /pics/Pipeline.png

![Pipeline DAG](pics/Pipeline.png)

# ▶️Instructions to Run

Start development container

Install dependencies

pip install -r requirements.txt

Initialize Airflow

airflow db init

Start Airflow

airflow scheduler & airflow webserver

Access Airflow UI: http://localhost:8080

Enable DAG pipeline