# SaaS Revenue & Churn Analytics Dashboard

An end-to-end SaaS analytics project that simulates how modern data teams transform raw operational data into executive-ready insights using PostgreSQL and Power BI.

This project covers the full analytics lifecycle from raw data ingestion and modeling to KPI engineering, dashboard design, and live deployment.

---

## 🔍 Project Overview

This dashboard is designed to help SaaS stakeholders answer critical business questions such as:

- Why are customers churning?
- How much revenue is being lost due to churn?
- Which features drive retention or risk?
- How do revenue and churn trends evolve over time?

The solution follows real-world analytics best practices used in SaaS organizations.

---

## 🧱 Data Sources

Raw data simulates fragmented SaaS data typically pulled from billing systems, product analytics, and CRM tools.

**Raw datasets (`/data/raw`):**
- `ravenstack_accounts.csv` - customer account details
- `ravenstack_subscriptions.csv` - subscription plans and pricing
- `ravenstack_feature_usage.csv` - product feature usage
- `ravenstack_churn_events.csv` - churn timestamps and churn reasons
- `ravenstack_support_tickets.csv` - support activity linked to churn risk

---

## 🗄️ Data Modeling & Transformation (PostgreSQL)

All raw datasets were ingested into **PostgreSQL** for transformation and metric engineering.

### Key work performed:
- Designed a relational schema using primary and foreign keys
- Joined customer, subscription, usage, churn, and support datasets
- Cleaned and standardized timestamps, pricing, and usage fields
- Engineered core SaaS business metrics

### Core metrics engineered:
- Active subscriptions
- Churn counts and churn rate (%)
- Monthly Recurring Revenue (MRR)
- Annual Recurring Revenue (ARR)
- Average revenue impact of churn
- Feature usage intensity
- Beta feature adoption signals

---

## 📦 Analytics Output

A denormalized, analytics-ready dataset was created to support BI consumption.

**Processed dataset:**
/data/processed/dashboard_master_view.csv

yaml
Copy code

This file represents a production-style analytics warehouse output optimized for dashboarding.

---

## 📊 Power BI Analytics & Dashboarding

The processed dataset was imported into **Power BI** to build a clean analytical data model.

### Data modeling:
- Fact-style analytical table optimized for slicing and filtering
- Business-friendly measures created using DAX

### DAX measures include:
- Churn Rate (%)
- MRR and ARR
- Average revenue impact
- Feature usage metrics
- Beta feature usage rate

---

## 📈 Dashboard Design

The dashboard was designed for **decision-making**, not just reporting.

### Key components:
- Executive KPI overview
- Churn trends and churn reason analysis
- Revenue trends over time
- Feature usage heatmap by plan tier
- Most-used and least-used feature identification
- Custom tooltip pages providing contextual insights on hover

---

## 🌐 Dashboard Publishing

The final Power BI dashboard was published online, enabling interactive access without requiring Power BI Desktop.

🔗 **Live Dashboard:**  
https://app.powerbi.com/reportEmbed?reportId=6b5810e6-e1dc-40bd-b3f2-8442d8e97ce8&autoAuth=true&ctid=4278a402-1a9e-4eb9-8414-ffb55a5fcf1e

This simulates real-world BI deployment for business stakeholders.

---

## 📂 Project Structure
```text
data/
├── raw/
│   ├── ravenstack_accounts.csv
│   ├── ravenstack_subscriptions.csv
│   ├── ravenstack_feature_usage.csv
│   ├── ravenstack_churn_events.csv
│   ├── ravenstack_support_tickets.csv
│   └── README.md
└── processed/
    └── dashboard_master_view.csv
```

## 🧠 Key Takeaways

This project demonstrates:

- End-to-end analytics ownership
- Strong SQL and relational data modeling skills
- Business-focused metric engineering
- Advanced Power BI and DAX capabilities
- Experience building executive-ready SaaS dashboards
- Realistic BI deployment workflows

The implementation closely reflects how analytics teams operate in modern SaaS organizations.

---

## 🛠️ Tools & Technologies

- **PostgreSQL** - data modeling and transformation
- **SQL** - joins, aggregations, metric engineering
- **Power BI** - dashboarding and DAX measures
- **GitHub** - version control and project documentation

---

## 👤 Author

**Yash Jadhav**  
MS in Computer Science  
SaaS Analytics | Data Analytics | Business Intelligence
