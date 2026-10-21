# Reliance Jio Network Experience & Service Reliability Intelligence Dashboard - 2026

## Project Information

**Project Title:**  
Reliance Jio Network Experience & Service Reliability Intelligence Dashboard - 2026

**Industry Name:**  
Telecom / Network Analytics

**Problem Statement:**  
Telecom companies need to continuously monitor network quality, service reliability, customer support performance, speed, and performance across different telecom circles. Analyzing these indicators helps identify performance trends, compare providers and circles, and understand areas that may require attention. This project uses publicly available telecom data to develop a Power BI-based analytics dashboard for analyzing network experience and service reliability in a structured and interactive way.

**Project Objectives:**

- Analyze telecom network availability and service reliability indicators.
- Monitor call setup and customer service performance.
- Analyze call-drop and packet-drop related measures.
- Compare network performance across telecom providers.
- Analyze performance across telecom circles.
- Study P80 download and upload speed trends.
- Compare speed and tariff-related information.
- Use MySQL and SQL for structured data storage and analysis.
- Use Power Query for data preparation and transformation.
- Use Power BI and DAX to create interactive analytical dashboards.
- Present business-oriented insights through KPIs, trends, comparisons and detailed tables.

**Proposed Solution / Business Questions:**

The project combines MySQL, SQL, Power Query, Power BI and DAX to convert public telecom performance data into an interactive business intelligence dashboard.

The analysis addresses questions such as:

- What is the overall network availability?
- How does network availability change over time?
- What is the call setup success performance?
- How does customer service performance vary across providers?
- How do call-drop and packet-drop indicators change by month?
- Which telecom circles show stronger or weaker network performance?
- How does P80 download speed vary across telecom circles?
- How do download and upload speeds change month by month?
- How do speed and tariff categories compare across telecom circles?
- How does Reliance Jio compare with other telecom providers in the available public dataset?

**Dataset Name:**  
Jio Telecom Network Performance Dataset

**Dataset Source:**  
TRAI Public Telecom Data

**Database Name:**  
jio_network

**Table Names:**  
Table 1: `fact_qos`  
Table 2: `fact_customer`  
Table 3: `fact_speed`

## Tools & Technologies

- MySQL
- SQL
- Power BI Desktop
- Power Query
- DAX
- CSV / Excel for dataset preparation and import

## Project Overview

This project focuses on telecom network experience and service reliability analysis using publicly available telecom data. The analysis examines network availability, call setup performance, customer service indicators, network speed, telecom circle performance, and tariff-related information.

The project uses MySQL and SQL for structured data storage and analysis, while Power Query, Power BI, and DAX are used for data preparation, modeling, KPI calculation, and interactive dashboard development.

The main purpose is to transform telecom performance data into meaningful visual insights that can help understand network quality, service reliability, provider performance, circle-wise differences, and speed trends. The project is developed for academic and analytical purposes and does not use private Reliance Jio internal data.

## Dataset Information

- **Dataset Name:** Jio Telecom Network Performance Dataset
- **Number of Rows:** 944 rows in `fact_qos`, 934 rows in `fact_customer`, and 1,000 rows in `fact_speed`
- **Important Features / Columns:**
  - Provider name and provider code
  - Telecom circle / LSA information
  - Month and reporting period
  - Network availability
  - Call setup / call service indicators
  - Call-drop indicators
  - Packet-drop indicators
  - Customer service indicators
  - P80 download speed
  - P80 upload speed
  - Tariff category
  - Speed-related measures

## Project Workflow

Industry Selection  
↓  
Problem Identification  
↓  
Dataset Collection  
↓  
MySQL Database Setup  
↓  
Data Cleaning & Transformation Using SQL  
↓  
SQL Data Analysis  
↓  
Power BI Data Modeling  
↓  
Dashboard Development  
↓  
Insights & Recommendations

## SQL Analysis

The following SQL statements were used to create/select the project database and inspect the imported tables:

```sql
CREATE DATABASE project;
USE project;
SELECT * FROM fact_qos;
SELECT * FROM fact_customer;
SELECT * FROM fact_speed;
```

These queries establish the database context and preview the imported table data. Additional SQL analyses are documented only where the corresponding queries are available in the project SQL files.

## Power BI Dashboard

The Power BI report contains three pages.

### 1. Network Performance Overview

Includes KPI cards for network availability, call setup success, average latency, and packet drop rate, along with visuals for network availability trends, monthly data call drops, monthly packet drop rate, P80 download speed by telecom circle, provider-wise network performance, and detailed provider/circle performance.

### 2. Customer Service & Reliability Analysis

Includes KPI cards for call center accessibility, calls answered within 90 seconds, bill resolution, bill complaints, and service closure within 7 days. It also includes a gauge for calls answered within 90 seconds, monthly provider ranking, customer support performance by provider, and Jio customer service performance by telecom circle.

### 3. Speed, Circle & Tariff Analysis

Includes monthly P80 download and upload speed trends, speed comparison across telecom circles and tariff categories, average P80 download speed by tariff category, and KPI cards for download and upload speed performance.

The Power BI report uses Power Query for data preparation and transformation, data modeling for analysis across the project tables, and DAX measures for KPI calculations. The dashboard also uses interactive filters and page navigation between the three analytical pages.

## Data Analysis & Visualization

The project performs:

- Network Performance Analysis
- Trend Analysis
- Telecom Circle Analysis
- Customer Service Analysis
- Reliability Analysis
- Speed Performance Analysis
- Download vs Upload Comparison
- Tariff Category Analysis
- Monthly Analysis
- KPI Analysis
- Provider Comparison
- Performance Comparison

The analysis is presented through KPI cards, trend charts, comparison visuals, gauge, scatter, ribbon, matrix, tables, and other implemented Power BI visuals.

## Key Insights

- Network availability and service quality indicators can be monitored through the overall network performance dashboard.
- Monthly trend visuals help identify changes in network availability, call-drop and packet-drop performance.
- Provider comparison visuals help understand differences in network and customer service performance.
- Circle-wise analysis helps identify variations in performance across telecom service areas.
- Customer service KPIs show the performance of accessibility, calls answered within 90 seconds, billing-related indicators, and service closure.
- Speed analysis helps identify differences in P80 download and upload performance across months, circles, and tariff categories.
- The dashboard provides a consolidated view of network experience, customer service, reliability, and speed-related indicators for business-oriented analysis.

These insights are based on the available project dataset and dashboard analysis and do not represent private or internal Reliance Jio operational results.

## Power BI Dashboard Screenshots

### Network Performance Overview

![Network Performance Overview](Screenshot/network_performance_overview.png)

### Customer Service & Reliability Analysis

![Customer Service & Reliability Analysis](Visualizations/customer_service_reliability_analysis.png)

### Speed, Circle & Tariff Analysis

![Speed, Circle & Tariff Analysis](Visualizations/speed_circle_tariff_analysis.png)

## Project Folder Structure

```text
Reliance-Jio-Network-Experience-Analytics/
│
├── README.md
│
├── Dataset/
│   ├── raw_dataset/
│   └── cleaned_dataset/
│
├── SQL/
│   ├── database_setup.sql
│   ├── data_cleaning.sql
│   └── data_analysis.sql
│
├── PowerBI/
│   └── jio_network_experience_dashboard.pbix
│
└── Visualizations/
    ├── network_performance_overview.png
    ├── customer_service_reliability_analysis.png
    └── speed_circle_tariff_analysis.png
```

## Author

- **Name:** Devika R
- **Student ID:** AF05331703
- **Organization:** Anudip Foundation
- **Course:** DBA_AI
- **Batch Code:** ANP-D7635

