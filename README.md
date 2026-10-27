# PySpark & Apache Airflow ETL Pipeline

A robust, production-grade data pipeline that orchestrates automated data ingestion, transformation using PySpark, and loading into a target data store.

## Architecture Overview
1. **Trigger:** Apache Airflow schedules and triggers the pipeline daily.
2. **Ingestion:** Pulls raw JSON/CSV logs from source storage.
3. **Transformation:** PySpark cleans, aggregates, and structures the data (handles nulls, computes metrics, partitions output).
4. **Load:** Saves optimized Parquet files ready for analytics.

## Project Structure
```text
spark-airflow-etl-pipeline/
├── dags/
│   └── customer_etl_dag.py
├── scripts/
│   └── transform_data.py
├── requirements.txt
└── README.md
