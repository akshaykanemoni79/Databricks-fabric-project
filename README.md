# Databricks-fabric-project
End-to-End E-commerce data lake house built with Databricks, Fabric, and Power BI. Features Medallion Architecture (Bronze-Silver-Gold), SCD Type 2 loyalty tracking, data quality validation, and analytics dashboards.
# 🛒 E-Commerce Medallion Architecture Project

An end-to-end Data Engineering lakehouse pipeline built using **Databricks**, **Microsoft Fabric**, **Power BI**, and **GitHub**. This project processes raw e-commerce transaction data, enforces automated data quality checks, implements **SCD Type 2** for customer loyalty tracking, and delivers business-ready analytics dashboards.

---
Project: E-Commerce Customer Loyalty Analytics

Tech Stack:
- GitHub
- Azure Databricks
- PySpark
- Delta Lake
- Medallion Architecture
- SCD Type 2
- Microsoft Fabric
- Power BI

Architecture:

GitHub
↓
Databricks Repos
↓
Bronze Layer
↓
Silver Layer
↓
Gold Layer
↓
Fabric Lakehouse
↓
Power BIks and assertions
├── scd_type2_loyalty.py       # Slowly Changing Dimension Type 2 implementation
├── gold.py                    # Business aggregations (Sales & Loyalty metrics)
└── README.md                  # Project documentation
