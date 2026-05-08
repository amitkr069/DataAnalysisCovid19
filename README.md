# Global COVID-19 Analytics Pipeline

## Project Overview

This project is an end-to-end data engineering and analytics pipeline built using PySpark. The goal was to take raw, fragmented COVID-19 datasets from multiple sources and transform them into clean, actionable insights.

Instead of just running basic queries, this project scales up into a fully automated ETL (Extract, Transform, Load) pipeline that cleans the data, calculates advanced metrics, and exports the final reporting tables (in CSV and Parquet formats) so they can be easily plugged into visualization dashboards like Tableau or Power BI.

---

## What This Pipeline Does

Data Cleaning & Standardization: Ingests six different datasets, infers schemas, handles missing values, and fixes naming inconsistencies (like unifying "US" and "USA") so the data can be accurately joined.

Global Aggregations: Calculates the top most affected countries, mortality rates, and overall case breakdowns by WHO regions.

Time-Series Tracking: Uses PySpark Window functions to track daily case growth, monthly trends, and pinpoint the exact peak days of the pandemic.

Geographic Analysis: Maps out US state-wise case distributions and identifies global infection clusters using Latitude and Longitude coordinates.

Advanced Feature Engineering: Calculates recovery rates, identifies "high-risk" countries where active cases outnumber recoveries, and dynamically categorizes countries into severity tiers (Low to Critical) based on infection volume.

Automated ETL Execution: The final script wraps all these steps into a modular, repeatable pipeline that processes the raw data and spits out clean, finalized reporting tables.

---

## Tech Stack Used

Big Data Processing: PySpark (Spark SQL, Window Functions, DataFrames)

Data Manipulation: Python, Pandas

Data Visualization: Matplotlib, Seaborn, Plotly
