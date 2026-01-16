🔄 End-to-End Analytics Workflow

This project was built as a full analytics pipeline, simulating how real SaaS companies transform raw operational data into executive dashboards.

1️⃣ Raw Data Ingestion

We started with multiple raw CSV datasets representing core SaaS business entities:

Accounts: customer metadata and churn flags

Subscriptions: plan tier, ARR, MRR, renewals

Feature Usage: product usage events and engagement depth

Churn Events: churn timing and reason codes

Support Tickets: operational signals tied to churn

These files are stored under:

/data/raw


The raw data mirrors how SaaS data typically arrives from different systems (billing, product analytics, support tools).

2️⃣ Data Modeling & Transformation (PostgreSQL)

All raw datasets were loaded into PostgreSQL for transformation and modeling.

Key steps:

Defined relational schema using primary and foreign keys

Joined subscriptions, usage, churn, and support data

Aggregated metrics such as:

Active subscriptions

Churn counts and rates

Revenue (MRR / ARR)

Feature usage intensity

Created a denormalized analytics view optimized for BI consumption

The final analytics-ready output was exported as:

/data/processed/dashboard_master_view.csv


This mirrors a real-world analytics warehouse view.

3️⃣ Power BI Data Modeling & Measures

The processed dataset was imported into Power BI.

Within Power BI:

Built a clean star-style data model

Created DAX measures for:

Churn Rate (%)

Average Revenue Impact

Feature Usage Metrics

Beta Feature Adoption Rate

Implemented:

KPI cards for executive overview

Time-series trend analysis

Feature usage heatmaps

Churn reason breakdowns

Custom tooltip pages for deeper insights

4️⃣ Interactive Dashboard Design

The dashboard was designed for business stakeholders, not just analysts.

Features include:

Executive KPI overview page

Product & feature analytics page

Custom tooltip pages explaining churn impact on hover

Clean labeling and short metric names for clarity

Plan-tier segmentation for deeper analysis

5️⃣ Publishing & Online Access

The final dashboard was published online to enable interactive access without Power BI Desktop.

🔗 Live Dashboard Link:
(Add your published Power BI Service link here)

This allows stakeholders to explore insights dynamically, simulating real-world BI deployment.

📂 Project Structure
data/
├── raw/                # Original SaaS datasets
├── processed/          # Analytics-ready output
│   └── dashboard_master_view.csv

🎯 Outcome

This project demonstrates:

End-to-end data analytics ownership

SQL-based data modeling and aggregation

Business-focused KPI design

Strong Power BI & DAX skills

Realistic SaaS analytics workflow

Built to reflect how analytics is actually done in production environments.
