# ⚖️ Task 2: Forensic Technology 

## Overview

This project was completed as part of the **Deloitte Data Analytics Job Simulation** on **Forage**.

The objective was to analyze employee compensation data and classify the level of gender pay equality across different factories and job roles using Microsoft Excel.

---

## Business Scenario

A manufacturing company, **Daikibo**, received internal complaints regarding potential gender pay inequality.

To support the investigation, Deloitte's Forensic Technology team generated an **Equality Score** for each combination of factory and job role. The task was to classify these scores into meaningful categories to help identify areas requiring further investigation.

---

## Tools Used

- Microsoft Excel
- IF Functions
- Logical Operators (AND)
- Data Classification

---

## Dataset

The dataset contained the following fields:

- **Factory**
- **Job Role**
- **Equality Score** (Range: -100 to +100)

An additional column, **Equality Class**, was created to classify each record based on its Equality Score.

---

## Classification Logic

The Equality Score was categorized into three classes:

| Equality Score | Classification |
|---------------:|----------------|
| Between **-10** and **10** (inclusive) | Fair |
| Greater than **10** or less than **-10** | Unfair |
| Greater than **20** or less than **-20** | Highly Discriminative |

### Excel Formula

```excel
=IF(OR(C2>20,C2<-20),"Highly Discriminative",
IF(OR(C2>10,C2<-10),"Unfair","Fair"))
```

> **Note:** `C2` refers to the **Equality Score** column.

---

## Key Skills Demonstrated

- Excel logical functions
- Nested IF statements
- AND / OR conditions
- Data classification
- Business rule implementation
- Forensic data analysis

---

## Deliverables

- Classified employee compensation dataset
- Excel formula implementation
- Equality classification for every factory and job role

---

## Learning Outcomes

Through this task, I gained practical experience in:

- Applying business rules using Excel formulas
- Building nested logical conditions
- Classifying data for forensic investigations
- Translating analytical requirements into automated Excel solutions
