# operational-performance-infrastructure-monitoring-analysis


**Excel** · **EDA**· **Power BI** · **DAX** · **Power Query** · **Data Modeling** · **Business Intelligence**

---
## 📖 Project Overview

A data-center operational performance and infrastructure monitoring dataset.


---

# 🎯 Business Problem

The Data Centre wants to understand **how efficiently and reliably is the data centers/assets operating, and which clients, assets, or conditions are driving high energy consumption, performance issues, or system alerts**

The analysis focuses on five key business areas.


### 1️⃣ Client Performance Analysis

How is the business performing over time?

* What is total revenue?
* How many units are being sold?
* How many sales transactions are occurring?
* How are sales changing over time?
* Which stores generate the most revenue?

---
### 2️⃣ Asset Utilization & Operational Health

How is the business performing over time?

* Which asset models consume the most power?
* Are older assets less efficient?
* Are certain assets generating more alerts?
* What is the total power consumed per asset compared to its total rated capacity (Capacity_kW)?
* Which Asset_Model runs at the highest average thermal reading (Thermal_Reading_C), and does it correlate with high CPU utilization?
  
  
---

### 3️⃣ Infrastructure Telemetry & Industry Analysis

How is the business performing over time?

* Which Industry accounts for the highest total power consumption (Power_Consumed_kWh)?
* Which asset models consume the most power?
* Which Industry accounts for the highest total power consumption (Power_Consumed_kWh)?
* What is the average CPU utilization (Avg_CPU_Utilization_Pct) per Contract_Tier?
* Who are the top 10 clients (Client_ID) generating the most system alerts (System_Alerts) across all their operational assets?

---

### 4️⃣ Regional & Portfolio Efficiency

* What is the total power consumption per HQ_Region (e.g., Nairobi East, Nairobi West, Kigali, Mombasa, Dar es Salaam)?
* Which regional clients experience the highest average number of system alerts per telemetry log?
* How does client contract tier (Contract_Tier) affect the average workload/CPU utilization placed on data center assets?
  
---

### 5️⃣ Risk & Maintenance Monitoring

* Which client-asset combinations are generating the highest total volume of System_Alerts?
* Are older assets (based on Installation_Date) generating significantly more thermal warnings or system alerts than newer installations?
* What percentage of total telemetry records register both high thermal readings (>30°C) and active system alerts (>0)?




# 🚀 Project Objectives

---



# 🛠 Tools Used

---
# 📂 Dataset Overview

The Maven Toys dataset contains multiple tables representing different aspects of the retailer's operations.

The project uses five main tables:

### `Client`

The table tells you who the data center customer is.

| Column           | Description                         |
| ---------------- | ----------------------------------- |
| `Client_ID`      | unique client                       |
| `Company_Size`   | the size of the company             |
| `Industry`       | healthcare, fintech, media, etc.    |
| `Contract_Tier`  | contract identifier                 |
| `HQ_Region`      | where the company is headquartered  |

---

### `Asset`

This describes the physical/technical infrastructure.

| Column                  | Description               |
| ----------------------- | ------------------------- |
| `Asset_ID`              | Unique asset identifier   |
| `Asset_Model`           | Type/model of asset       |
| `Capacity_kW`           | How much power it is designed to handle        |
| `Installation_Date`     | How old it is          |
| `Operational_Status`    | is it operating    |

---

### `Infrastructure_Telemetry`

It contains measurements over time. This is where you can actually **measure performance and operational behavior over time**.

| Column                  | Description               |
| ----------------------- | ------------------------- |
| `Telemetry ID`              | Unique observation   |
| `Date ID`           | When the measurement occurred      |
| `Client_ID`           | Unique client identifier        |
| `Asset_ID`     | Unique asset identifier          |
| `Power_Consumed_kWh`    | Energy/power usage    |
| `Avg_CPU_Utilization_Pct`     | How heavily the system is being used          |
| `Thermal_Reading_C`    | Temperature   |
| `Asset_ID`     | How old it is          |
| `System_Alerts`    | Whether an issue/alert occurred    |

---

# 🧹 Data Preparation


