# E-Commerce Sales Data Warehouse

A complete **Data Engineering** project that demonstrates the design and implementation of an ETL pipeline and a PostgreSQL-based data warehouse for e-commerce analytics. The project extracts data from the Fake Store API, transforms it into a structured format, loads it into a star schema data warehouse, and generates business insights using SQL and Python visualizations.

---

## Overview

This project follows the complete ETL (Extract, Transform, Load) workflow commonly used in modern data engineering. It showcases data ingestion from REST APIs, data cleaning, warehouse modeling, SQL analytics, and reporting.

The objective is to convert raw e-commerce data into a structured analytical database that supports efficient business reporting and decision-making.

---

## Features

* Automated data extraction from the Fake Store API
* Data cleaning and transformation using Python
* PostgreSQL Data Warehouse implementation
* Star Schema design for analytical workloads
* SQL queries for business intelligence
* Python-based visualizations and reporting
* Modular ETL pipeline
* Well-documented project structure

---

## Technologies Used

* Python
* PostgreSQL
* SQL
* Pandas
* Requests
* Matplotlib
* REST API
* Git & GitHub

---

## Project Structure

```text
E-commerce-Sales-Warehouse/
│
├── README.md
├── requirements.txt
├── LICENSE
├── .gitignore
│
├── data/
│   ├── raw/
│   └── processed/
│
├── scripts/
│   ├── ingestion.py
│   ├── transformation.py
│   ├── modeling.py
│   └── stats.py
│
├── sql/
│   ├── staging_schema.sql
│   ├── dw_schema.sql
│   └── queries.sql
│
├── config/
│   ├── db_config.json
│   └── api_config.json
│
├── notebooks/
│   └── exploration.ipynb
│
└── reports/
    ├── images/
    ├── final_report.pdf
    └── stats_report.md
```

---

# ETL Pipeline

## 1. Data Extraction

The project extracts data from the Fake Store API.

Datasets include:

* Products
* Users
* Carts
* Categories

The extracted JSON files are stored inside:

```text
data/raw/
```

---

## 2. Data Transformation

The transformation process includes:

* Cleaning missing values
* Flattening nested JSON
* Standardizing column names
* Data type conversion
* Removing duplicate records
* Creating analysis-ready datasets

The processed files are stored in:

```text
data/processed/
```

---

## 3. Data Warehouse Design

A PostgreSQL data warehouse is designed using a **Star Schema**.

### Fact Table

* Sales Fact

### Dimension Tables

* Product Dimension
* User Dimension
* Category Dimension
* Cart Dimension

This schema enables efficient analytical queries and reporting.

---

## Business Insights

Example analyses include:

* Total sales by category
* Highest-priced products
* Customer purchasing behavior
* Product ratings analysis
* Category-wise product distribution
* Order trends
* Revenue analysis

Business insights are generated using SQL queries and Python visualizations.

---

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/saitejaravi2300/E-commerce-Sales-Warehouse.git
```

### Navigate to the Project

```bash
cd E-commerce-Sales-Warehouse
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Configure Database

Update the PostgreSQL credentials inside:

```text
config/db_config.json
```

If required, modify:

```text
config/api_config.json
```

---

## Run the ETL Pipeline

Execute the scripts in the following order:

```bash
python scripts/ingestion.py
python scripts/transformation.py
python scripts/modeling.py
```

---

## Generate Reports

```bash
python scripts/stats.py
```

This script generates:

* SQL-based analytical reports
* Business insights
* Charts and visualizations

---

## Sample Business Questions Answered

* Which product categories generate the highest sales?
* Which products have the highest ratings?
* Which users purchase the most products?
* What are the purchasing trends across categories?
* How is product distribution spread across categories?

---

## Learning Outcomes

This project demonstrates practical experience with:

* ETL Pipeline Development
* Data Engineering
* REST API Integration
* PostgreSQL Database Design
* Star Schema Modeling
* SQL Analytics
* Data Cleaning
* Python Automation
* Data Visualization
* Business Intelligence

---

## Future Enhancements

* Incremental ETL loading
* Workflow orchestration using Apache Airflow
* Docker containerization
* Cloud deployment (AWS/GCP/Azure)
* Interactive Power BI Dashboard
* Automated scheduling and monitoring

---

## License

This project is licensed under the Apache License 2.0.

---

## Author

**Ravi Sai Teja**

GitHub: https://github.com/saitejaravi2300

LinkedIn: *([https://www.linkedin.com/in/saiteja-ravi-a72a6b291/])*

---

## Acknowledgements

This project uses the public **Fake Store API** as the data source for educational and analytical purposes.
