## 📊 Task 1: Data Analysis

## Overview

This project was completed as part of the **Deloitte Data Analytics Job Simulation** on **Forage**.

The objective was to analyze telemetry data collected from multiple manufacturing facilities using **Tableau** to identify operational downtime and determine which factory and machine types experienced the highest number of failures.

---

## Business Scenario

A manufacturing company, **Daikibo**, collected telemetry data from machines across four factories over one month. Each machine reported its operational status every 10 minutes.

The analysis aimed to answer the following business questions:

1. Which factory experienced the highest machine downtime?
2. Which machine types contributed the most to downtime at that factory?

---

## Tools Used

- Tableau
- JSON Dataset
- Calculated Fields
- Interactive Dashboards
- Data Visualization

---

## Approach

### 1. Data Import

- Imported the telemetry dataset into Tableau.
- Verified all schema levels during data import to ensure the dataset was loaded correctly.

### 2. Data Preparation

Created a calculated field named **Unhealthy** to measure machine downtime.

```text
IF [Status] = "unhealthy" THEN 10 ELSE 0 END
```

Each unhealthy status represented **10 minutes** of downtime since the previous telemetry message.

### 3. Factory-Level Analysis

Created a bar chart to visualize the total downtime for each factory.

**Visualization**
- Down Time per Factory

### 4. Device-Level Analysis

Created another bar chart showing downtime by machine type.

**Visualization**
- Down Time per Device Type

### 5. Interactive Dashboard

Combined both visualizations into a dashboard.

Configured the dashboard so that selecting a factory automatically filters the machine-level visualization, allowing focused analysis of downtime within that factory.

---

## Key Skills Demonstrated

- Data visualization
- Tableau dashboard development
- Calculated fields
- Manufacturing data analysis
- Interactive filtering
- Business insight generation

---

## Deliverables

- Tableau dashboard
- Factory downtime analysis
- Machine type downtime analysis
- Interactive filtering dashboard

---

## Screenshots

### Dashboard

> ![Dashboard](Task1_Dashboard_screenshot.png)

> <img width="1920" height="1028" alt="Task1_Dashboard" src="https://github.com/user-attachments/assets/bfadda22-9daa-42d6-8a8e-34357d6daa97" />

---

## Learning Outcomes

Through this project, I gained hands-on experience with:

- Importing and preparing JSON data in Tableau
- Creating calculated measures
- Building interactive dashboards
- Transforming telemetry data into actionable business insights
- Communicating findings through visual analytics
