# Online Retail Analysis – Databricks (PySpark)

## Overview

This project performs large-scale transactional data analysis on an Online Retail dataset using PySpark on Databricks.

The objective is to clean raw retail data, handle inconsistencies, and extract business insights such as top-selling products, revenue distribution, cancellation trends, and country-wise sales performance.

## Tech Stack

Platform: Databricks Workspace

Engine: Apache Spark (PySpark)

Language: Python

Data Storage: Databricks Catalog

Dataset: Online Retail transactional dataset

## Dataset Columns

1. InvoiceNo
2. StockCode
3. Description
4. Quantity
5. InvoiceDate
6. UnitPrice
7. CustomerID
8. Country
Each row represents a product-level transaction.

## Project Workflow

1️⃣ Data Ingestion

Loaded CSV into Spark DataFrame

Enabled header and schema inference

Verified schema and record counts

2️⃣ Data Cleaning

Removed duplicates

Filtered invalid transactions (Quantity <= 0, UnitPrice <= 0)

Separated cancelled invoices (InvoiceNo starting with “C”)

Handled null values

Casted appropriate data types

3️⃣ Feature Engineering

Created TotalPrice = Quantity × UnitPrice

## Analysis Performed

1. Total valid vs cancelled transactions

2. Top-selling products (by quantity)

3. Top revenue-generating products

4. Most frequently purchased items

5. High-frequency but low-revenue products

6. Revenue by country

## Key Insights

1. Identified high-demand and high-revenue products

2. Analyzed cancellation patterns

3. Evaluated geographical revenue distribution

4. Built a clean dataset ready for advanced analytics

## Future Enhancements

1. Customer segmentation (RFM analysis)

2. Time-series sales trends

3. Predictive modeling

4. Dashboard integration (Power BI / Tableau)

## Outcome

This project demonstrates scalable data processing and business analytics using PySpark on Databricks, converting raw retail transactions into actionable insights.
