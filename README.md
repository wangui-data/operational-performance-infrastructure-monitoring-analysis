# operational-performance-infrastructure-monitoring-analysis


**Excel** · **EDA**· **Power BI** · **DAX** · **Power Query** · **Data Modeling** · **Business Intelligence**

---
## 📖 Project Overview

a data-center operational performance and infrastructure monitoring dataset.


---

# 🎯 Business Problem

The Data Centre wants to understand **how efficiently and reliably is the data centers/assets operating, and which clients, assets, or conditions are driving high energy consumption, performance issues, or system alerts**

The analysis focuses on five key business areas.

---

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


