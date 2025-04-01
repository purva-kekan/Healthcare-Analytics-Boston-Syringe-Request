# 🧪 Boston 311 Syringe Requests – Predictive Analytics & Geospatial Insights

> 🚫 **Note:** This project contains sensitive data and analysis developed for a specific stakeholder.  
> As such, the repository is **private** and **not publicly shareable** due to confidentiality agreements.

---

## 📌 Project Overview

This project works on **predictive analytics** and **geospatial data** to analyze and visualize the distribution of **Boston 311 syringe service requests** from 2011 to 2025. The goal is to identify spatial disparities in municipal service delivery and forecast future trends to help Boston Public Works allocate resources equitably and efficiently.

It is a part of a broader **equity-focused public health initiative** aimed at improving outcomes in underserved communities through data-driven strategies.

---

## 🎯 Objectives

- Analyze historical syringe service request trends by neighborhood, time, and request type.
- Identify geographic hotspots of high demand and SLA non-compliance.
- Evaluate the impact of the **Community Service Redemption Program (CSRP)** using time-series forecasting.
- Develop interactive **Power BI dashboards** to guide decision-makers.

---

## 📁 Data Source

- **Boston 311 Service Requests Dataset** (3M+ records from 2011 to 2025)  
  Source: [Analyze Boston](https://data.boston.gov/dataset/311-service-requests)

---

## 🧹 Data Processing & Feature Engineering

- Merged yearly datasets into a unified dataframe
- Dropped irrelevant columns and standardized data types
- Imputed missing values (e.g., `sla_target_dt`, `closed_dt`) using custom calculations
- Geocoded latitude/longitude and joined shapefiles for spatial mapping
- Filtered to only include **Syringe/Needle Pickup** requests (~65K records)
- Created SLA compliance measures and policy impact indicators

---

## 📊 Tools & Technologies

- **Python**: `pandas`, `numpy`, `matplotlib`, `seaborn` for data wrangling and analysis
- **Power BI**: Interactive dashboards for visualization and stakeholder reporting
- **Machine Learning**: SARIMA model for time-series forecasting

---

## 📈 Dashboard Highlights

- **Geospatial Analysis**: Heatmaps show service request clusters by neighborhood (e.g., Roxbury, South End)
- **Seasonal Trend Dashboard**: Tracks syringe requests over time (daily, monthly, yearly trends)
- **District-Level Breakdown**: SLA compliance, request frequency by district and ward
- **Forecasting Dashboard**: Compares actual vs. projected requests post-CSRP policy implementation

> 🔍 Dashboard Screenshots are available in the project folder as a PDF (`Boston311_SyringeRequest_Dashboard_PDF.pdf`)

---

## 🔬 Key Insights

- **Roxbury** had the highest volume of requests (>16,000), with notable hotspots in South End and Dorchester
- Most neighborhoods show high SLA compliance (~100%), though certain clusters had overdue cases
- A **significant rise** in requests occurred during the COVID-19 pandemic (2020)
- Post-2020 **CSRP policy** implementation helped stabilize or slightly reduce syringe request volumes

---

## 🤖 Forecasting Model

Used **SARIMA (Seasonal ARIMA)** to model and predict syringe request trends:
- Visualizes impact of CSRP policy using pre/post data comparisons
- Shows actual requests dipping below forecasted values post-policy, indicating positive program impact

---

---

## 🔒 Confidentiality Notice

This repository is **private** and developed as part of a **confidential group project** for academic and stakeholder purposes. Due to the nature of the data and sponsor involvement, **the content cannot be made public**.

---
