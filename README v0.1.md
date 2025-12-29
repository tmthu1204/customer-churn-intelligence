# Customer Churn Intelligence

## Overview
This project aims to build an **end-to-end Customer Churn Intelligence system**, focusing not only on predicting customer churn but also on **understanding the key behavioral drivers behind churn and translating data insights into actionable business recommendations**.

The project is designed to simulate a real-world data science workflow, covering the full pipeline from raw transactional data ingestion to analytics, machine learning, and decision support.

---

## Business Problem
Customer churn is a critical business challenge that directly impacts revenue and growth.  
Instead of solely answering *“Who will churn?”*, this project addresses three core business questions:
g
1. **Who** are the customers most likely to churn?
2. **Why** do these customers churn?
3. **What** actions can the business take to reduce churn?

---

## Dataset
The project uses a real-world **transactional retail dataset** (Online Retail II), which represents customer purchase logs over time.

**Key characteristics of the dataset:**
- Transaction-level data (raw event logs)
- Time-based purchase records
- Multiple customers, products, and geographic regions
- No predefined churn label (to reflect real-world scenarios)

This dataset is intentionally treated as **raw production data**, requiring feature engineering and business assumptions to define churn.

---

## Churn Definition (Target Variable)
Since churn is not explicitly provided, it is defined based on customer behavior:

> **A customer is considered churned if they have no purchase activity within the last _N_ days of the observation window.**

- The churn threshold (_N_) will be validated through exploratory analysis.
- This assumption reflects common industry practices in retail and subscription-like businesses.

---

## Project Scope
The project covers the following components:

- **Data Ingestion & ETL**
  - Raw data extraction
  - Data cleaning and validation
  - Feature generation and aggregation
  - Loading into a relational database

- **Data Modeling**
  - Fact and dimension tables (star schema)
  - SQL-based feature extraction

- **Exploratory Data Analysis (EDA) & Statistics**
  - Customer behavior analysis
  - Distribution and correlation analysis
  - Hypothesis testing to identify churn drivers

- **Machine Learning**
  - Classical ML models for churn prediction
  - Customer segmentation
  - Model evaluation and comparison

- **Visualization & Insights**
  - KPI dashboards
  - Churn and segment-level insights
  - Actionable business recommendations

---

## Project Architecture
```

Raw Transaction Data
↓
ETL Pipeline (Python)
↓
Relational Database (SQL)
↓
EDA & Statistical Analysis
↓
Machine Learning Models
↓
Insights & PowerBI Dashboard

```

---

## Expected Outcomes
- Identification of high-risk churn customer segments
- Understanding of key behavioral and transactional churn drivers
- A reproducible data science pipeline suitable for real-world deployment
- Clear, data-driven recommendations to support business decisions

---

## Technology Stack
- **Programming:** Python
- **Data Processing:** Pandas, NumPy
- **Database & SQL:** SQLite / PostgreSQL
- **Machine Learning:** Scikit-learn
- **Visualization:** PowerBI
- **Version Control:** Git & GitHub

---

## Project Status
🚧 **In Progress**  
This README represents **version 0.1**, focusing on problem definition, scope, and architecture.  
Subsequent updates will include implementation details, modeling results, and insights.
```g