# POWER-BI-Project-on-Marketing-Campaign-Performance
# 📊 Marketing Campaign Performance Dashboard | Power BI

## 📌 Project Overview

This project is an interactive **Marketing Campaign Performance Dashboard** built using **Microsoft Power BI**.

The dashboard analyzes marketing campaign data to understand campaign performance, customer engagement, channel effectiveness, geographic performance, conversion rates, ROI, clicks, impressions, and acquisition costs.

The project demonstrates practical skills in:

- Data Cleaning
- Data Modeling
- Data Transformation
- DAX
- KPI Development
- Interactive Dashboard Design
- Marketing Analytics
- Business Intelligence

---

## 🎯 Project Objective

The main objective of this project is to analyze marketing campaign performance and provide a clear view of:

- Overall campaign performance
- Marketing channel effectiveness
- Customer and audience behavior
- Geographic campaign performance
- Campaign ROI
- Click-through rate (CTR)
- Conversion rate
- Customer acquisition cost
- Monthly marketing trends

The dashboard allows users to filter the analysis by different campaign attributes and time periods.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Power BI Desktop** | Dashboard development and visualization |
| **Power Query** | Data cleaning and transformation |
| **DAX** | Measures, KPIs and time-based analysis |
| **Excel / CSV** | Source data |
| **Data Modeling** | Relationships between fact and dimension tables |

---

## 📂 Dataset

The dataset contains marketing campaign information such as:

- Campaign ID
- Campaign Type
- Channel Used
- Customer Segment
- Target Audience
- Location
- Language
- Campaign Date
- Impressions
- Clicks
- Conversion Rate
- Engagement Score
- Acquisition Cost
- ROI

The dataset contains approximately **200,000 campaign records**.

---

# 🧹 Data Preparation

The dataset was prepared using **Power Query** before creating the dashboard.

### Main data preparation steps

- Checked column data types
- Standardized date fields
- Reviewed missing values
- Removed/handled unnecessary fields
- Standardized categorical values
- Prepared numerical columns for analysis
- Created a structured data model
- Created a dedicated Date table for time-based analysis

---

# 🏗️ Data Modeling

A **star-schema-style data model** was used to organize the marketing data.

### Fact Table

**Fact_Marketing**

Contains the main transactional/campaign-level data:

- Campaign ID
- Date
- Impressions
- Clicks
- Conversion Rate
- Engagement Score
- Acquisition Cost
- ROI
- Campaign attributes


<img width="1330" height="749" alt="Screenshot 2026-09-21 131208" src="https://github.com/user-attachments/assets/fcf0f479-3a7d-43b9-b9f7-b38ae4f5fab7" />
<img width="1327" height="747" alt="Screenshot 2026-09-21 131239" src="https://github.com/user-attachments/assets/b4077481-f3fa-4eb6-aca1-251b52ef6547" />
<img width="1328" height="747" alt="Screenshot 2026-09-21 131305" src="https://github.com/user-attachments/assets/d1c8804d-8761-41e7-bb4b-96dbbdc78e98" />
<img width="1333" height="751" alt="Screenshot 2026-09-21 131338" src="https://github.com/user-attachments/assets/1f6db2f6-fa49-4fa3-8140-36a102a08064" />
<img width="1328" height="749" alt="Screenshot 2026-09-21 131401" src="https://github.com/user-attachments/assets/1676c53f-e0ad-43a4-9851-318db778e522" />


### Dimension Tables

- **Dim_Date**
- **Dim_Campaign**
- **Dim_Channel**
- **Dim_Location**

### Model Structure

```text
                  Dim_Date
                     │
                     │
                     ▼
Dim_Campaign ──► Fact_Marketing ◄── Dim_Channel
                     ▲
                     │
                     │
                Dim_Location


