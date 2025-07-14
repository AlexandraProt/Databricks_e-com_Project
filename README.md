# Databricks_e-com_Project
# 🛒 Cohort Retention Analysis with Fivetran & Databricks

This project demonstrates how to build a modern marketing analytics solution using the **modern data stack** — from data ingestion to cohort visualization — to analyze **customer retention behavior** in an e-commerce setting.

## 🎯 Objective

- Ingest e-commerce sales data from a **GCP Cloud SQL** database using **Fivetran**.
- Transform and model the data with **Databricks + Delta Lake**.
- Perform **cohort analysis** to understand retention patterns and time to second purchase.
- Visualize key trends using **Databricks Dashboards**.

## 🧱 Tools & Tech

- **Fivetran** – data ingestion from GCP Cloud SQL
- **Databricks** – data transformation, modeling, and visualization
- **Delta Lake** – for efficient storage and query performance
- **SQL & Python (pyspark.sql)** – for data processing
- **Databricks Dashboards** – for business insights

## 📊 Key Business Questions

- How many new customers are acquired each month (cohort size)?
- What is the time to second purchase for each cohort?
- How does retention change over time across different customer acquisition months?

## 📈 Key Insights

- The largest customer acquisition occurred in **January 2024** with **66 new users**.
- Subsequent months show a **decreasing trend** in new customer acquisition.
- Time to second purchase varies across cohorts, with **some cohorts showing longer retention gaps**, indicating potential areas for improvement in re-engagement strategies.

## 🖼️ Visuals

| Cohort Size by Month | Time to Second Purchase |
|----------------------|--------------------------|
| ![Cohort Size](./screenshots/cohort_size.png) | ![Time to Second Purchase](./screenshots/time_to_second_purchase.png) |

> 📍 All visuals are available in the [notebook](./notebooks/Explore_cohort_analysis_bigquery_catalog.cohort_db.ecom_orders.ipynb) and Databricks dashboard.


