# SaaS Revenue & Churn Analytics Dashboard

An end-to-end **SaaS analytics project** that transforms raw operational data into an interactive, executive-ready business intelligence dashboard using **PostgreSQL** and **Power BI**.

---

## 📌 Project Objective

The objective of this project is to design and implement a **real-world SaaS analytics pipeline** that answers key business questions around:

- Customer churn and retention
- Revenue performance (MRR / ARR)
- Product feature adoption
- Plan-tier behavior and usage patterns

This project simulates how analytics teams build dashboards used by **product managers, growth teams, and executive leadership**.

---

## 🗂️ Data Sources

The project uses multiple structured datasets representing core SaaS systems:

- **Accounts** – customer metadata and churn indicators  
- **Subscriptions** – plan tiers, pricing, MRR, ARR, renewals  
- **Feature Usage** – product usage events and engagement metrics  
- **Churn Events** – churn timestamps and churn reasons  
- **Support Tickets** – operational signals linked to churn risk  

All raw datasets are stored in:


/data/raw
These datasets intentionally mirror fragmented data typically pulled from billing platforms, product analytics tools, and CRM systems.

🧱 Data Modeling & Transformation (PostgreSQL)
All raw datasets were ingested into PostgreSQL for data cleaning, joins, and metric engineering.

Key work performed:
Designed a relational schema with primary and foreign keys

Joined customer, subscription, usage, churn, and support datasets

Engineered core SaaS business metrics including:

Active subscriptions

Churn counts and churn rate

Monthly Recurring Revenue (MRR)

Annual Recurring Revenue (ARR)

Feature usage intensity

Beta feature adoption signals

Created a denormalized analytics view optimized for BI consumption

The final analytics-ready dataset was exported as:

text
Copy code
/data/processed/dashboard_master_view.csv
This file represents a production-style analytics warehouse output.

📊 Power BI Analytics & Dashboarding
The processed dataset was imported into Power BI for data modeling and visualization.

Data Modeling & Measures
Built a clean analytical data model

Created DAX measures for:

Churn Rate (%)

Revenue metrics (MRR / ARR)

Average revenue impact

Feature usage metrics

Beta feature usage rate

Dashboard Design
The dashboard was designed for decision-making, not just reporting.

Key components include:

Executive KPI overview

Churn trends and churn reason analysis

Revenue trends over time

Feature usage heatmap by plan tier

Most-used and least-used feature identification

Custom tooltip pages providing contextual insights on hover

🌐 Dashboard Publishing
The final Power BI dashboard was published online, enabling interactive access without requiring Power BI Desktop.

🔗 Live Dashboard:
https://app.powerbi.com/reportEmbed?reportId=6b5810e6-e1dc-40bd-b3f2-8442d8e97ce8&autoAuth=true&ctid=4278a402-1a9e-4eb9-8414-ffb55a5fcf1e

This simulates real-world BI deployment for business stakeholders.

📁 Project Structure
text
Copy code
data/
├── raw/
│   ├── ravenstack_accounts.csv
│   ├── ravenstack_subscriptions.csv
│   ├── ravenstack_feature_usage.csv
│   ├── ravenstack_churn_events.csv
│   ├── ravenstack_support_tickets.csv
│   └── README.md
├── processed/
│   └── dashboard_master_view.csv
✅ Key Takeaways
This project demonstrates:

End-to-end analytics ownership

Strong SQL and relational data modeling skills

Business-focused metric engineering

Advanced Power BI and DAX capabilities

Experience building executive-ready SaaS dashboards

The implementation closely reflects how analytics teams operate in modern SaaS organizations.

🚀 Tools & Technologies
PostgreSQL – data modeling and transformation

SQL – joins, aggregations, metric engineering

Power BI – dashboarding and DAX measures

GitHub – version control and project documentation

📌 Author
Yash Jadhav
MS in Computer Science
SaaS Analytics | Data Analytics | Business Intelligence
