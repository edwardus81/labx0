# Data Engineering Day 2 Course

## Overview
This project covers a one-day crash course in data engineering using Python, focusing on Pandas, PySpark, Delta Lake, SQL, and ETL pipelines with the Wine Quality dataset.

## Tasks Completed
- **Pandas**: Normalized the Wine Quality dataset (`day2_course.ipynb`).
- **PySpark and Delta Lake**: Loaded data, analyzed it, and saved Delta tables (`local_pyspark.ipynb`).
- **SQL + ETL Pipeline**: Queried Delta tables and built an ETL pipeline to extract high-quality wines, transform with normalized alcohol, and load into a new Delta table.
- **Delta Lake Comparison**: Explored how Delta tables (used in PySpark/Databricks) compare to Pandas workflows, identifying Parquet and manual versioning as lightweight alternatives for small-scale data in Jupyter.

## File Structure
- `jup/`: Jupyter notebooks (`day2_course.ipynb`, `local_pyspark.ipynb`).
- `db/`: Databricks notebook (`winequality_analysis.ipynb`).
- `delta/`: Delta tables (`winequality-red/`, `high_quality_wines/`).
- `winequality-red.csv`: Source dataset.

## Challenges and Solutions
- **Issue**: Delta Lake/Parquet column naming restrictions (no spaces).
- **Solution**: Renamed columns (e.g., `fixed acidity` to `fixed_acidity`) before saving.

## Next Steps
- Explore advanced PySpark features (e.g., window functions).
- Build more complex ETL pipelines.
- Experiment with tools like SQLite, Dask, or Polars to enhance Pandas workflows.