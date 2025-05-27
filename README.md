# Superstore_DataEngineering_AWS_Project
End-to-End AWS Data Engineering Project

## Context
This project demonstrates how to build a **data pipeline** and perform **data analysis** on Superstore sales data using popular AWS services.It is ideal for beginners in **cloud data engineering**

---

## 📊 Project Objective

The goal is to build a **fully functional data pipeline** to:
- Ingest sales data to the cloud
- Perform ETL operations using Glue and PySpark
- Query processed data using Athena
- Visualize insights on QuickSight dashboards

---

## 🧰 Tools & AWS Services Used

| Component        | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| **Amazon S3**     | Used as the data lake to store raw and transformed data                    |
| **AWS Glue**      | Serverless ETL service to crawl, clean, and transform data with PySpark     |
| **AWS Athena**    | Serverless SQL query engine to analyze data in S3 using standard SQL        |
| **AWS IAM**       | Used for securely managing users, roles, and permissions                    |
| **AWS QuickSight**| Business Intelligence (BI) service for interactive dashboards and insights  |
| **Amazon CloudWatch** | (Optional) Logging and monitoring ETL jobs                              |

---

## 🧱 Project Architecture

              +----------------------+
              |   Local CSV Dataset  |
              +----------+-----------+
                         |
                         ↓
               Upload to Amazon S3 (Raw Zone)
                         |
                         ↓
            AWS Glue Crawler → Creates Table in Glue Catalog
                         |
                         ↓
              AWS Glue Job (PySpark ETL Script)
                         ↓
             Write Cleaned Data to S3 (Processed Zone)
                         ↓
                   Query via AWS Athena
                         ↓
               Visualize via AWS QuickSight











