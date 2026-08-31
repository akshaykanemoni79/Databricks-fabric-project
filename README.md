# Databricks-fabric-project
End-to-End E-commerce data lake house built with Databricks, Fabric, and Power BI. Features Medallion Architecture (Bronze-Silver-Gold), SCD Type 2 loyalty tracking, data quality validation, and analytics dashboards.
# 🛒 E-Commerce Medallion Architecture Project

An end-to-end Data Engineering lakehouse pipeline built using **Databricks**, **Microsoft Fabric**, **Power BI**, and **GitHub**. This project processes raw e-commerce transaction data, enforces automated data quality checks, implements **SCD Type 2** for customer loyalty tracking, and delivers business-ready analytics dashboards.

---

## 📐 Project Architecture
[ GitHub Repository ]
│
▼
[ Databricks Repos ]
│
┌─────────┴─────────┐
│    BRONZE LAYER   │  ──► Raw Ingestion + Metadata Tracking
└─────────┬─────────┘
│
┌─────────┴─────────┐
│    SILVER LAYER   │  ──► Data Cleansing, Deduplication & Validation
└─────────┬─────────┘
│
┌─────────┴─────────┐
│    GOLD LAYER     │  ──► Business Aggregations & SCD Type 2 Loyalty Tracking
└─────────┬─────────┘
│
▼
[ Microsoft Fabric ]  ──► Delta Lakehouse Integration
│
▼
[ Power BI Reports ] ──► Executive Dashboards & Analytics


---

## 📂 Repository Structure

```text
ecommerce-medallion-project/
│
├── sample data/               # Source CSV datasets
│   ├── customers.csv          # Customer profile data
│   ├── products.csv           # Product catalog and pricing
│   ├── orders.csv             # Raw transactional order data
│   └── loyalty_points.csv     # Loyalty rewards and tiers
│
├── bronze.py                  # Ingestion pipeline to Bronze Delta tables
├── silver.py                  # Cleansing, transformation, and deduplication
├── validation.py              # Automated data quality checks and assertions
├── scd_type2_loyalty.py       # Slowly Changing Dimension Type 2 implementation
├── gold.py                    # Business aggregations (Sales & Loyalty metrics)
└── README.md                  # Project documentation
