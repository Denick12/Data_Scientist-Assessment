# Data Scientist Technical Assessment

---

##  Overview

This repository contains my solutions to the **Data Scientist Technical Assessment**, completed using **Files 1–7** provided by the interviewer. The assessment evaluates skills in:

* Data ingestion and preparation
* SQL querying and analytical reasoning
* Time series forecasting using Python
* Statistical analysis and interpretation
* Logical reasoning and pattern recognition

The work is structured into clear sections aligned with the assessment questions.

---

## Repository Structure

```
├── Question 1 Solution/
│   └── merge_data.py          # Python script to merge Files 1–7
├── SQL_Queries/
│   └── queries.sql            # SQL queries answering questions 2–8
├── Forecasting/
│   ├── forecasting.ipynb      # Python notebook for time-series modeling
│   └── forecast_plot.png      # Visualization of actual vs forecasted calls
├── Results/
│   └── summary_tables.xlsx    # Output tables used in analysis
└── README.md                  # Project documentation (this file)
```

---

##  Section A – Data Preparation

### **Question 1: Combine Files 1–7**

* A Python script (`merge_data.py`) was developed using **Pandas** to combine the seven Excel files into a single dataset.
* Data cleaning steps included:

  * Standardizing column names
  * Handling missing values
  * Ensuring consistent data types
* The final output was exported as a **CSV file**, suitable for direct upload into a SQL database.
* The combined dataset was uploaded into SQL using **DBeaver**.

---

## Section B – SQL Analysis

SQL queries were written to analyze the full time period covered by Files 1–7.

Questions answered:
2. Count of unique users
3. Top 10 users by total calls handled
4. Average total handle time per call
5. Top 10 users by ratio of **peer disconnects** to total calls and comparison with other disconnect types
6. Monthly inbound queue calls
7. Percentage difference in inbound queue calls between 2023 and 2024
8. Month and year with the highest inbound queue volume

All queries are reproducible and included in the `SQL_Queries` on the Qestion 2-17 folder.

---

## Section C – Forecasting (Python)

### **Questions 9–13**

* Monthly call volumes for **2023 and 2024** were aggregated using Python.
* A **Holt-Winters Exponential Smoothing (ETS)** model with additive trend and seasonality was used to forecast call volumes for:

  * **2025**
  * **2026**

#### Model Justification

* Captures both **trend and seasonality**, which are evident in call volume data
* Performs well for short-to-medium term forecasting
* Interpretable and robust for operational forecasting

A visualization comparing **actual vs forecasted calls** is included in the repository.

---

## Section D – Statistical & Analytical Insights

### **Questions 14–17**

* **Hold Time vs Handle Time:** Strong positive correlation, indicating longer holds increase overall handling duration.
* **Talk Time vs Hold Time:** Talk time increases as hold time increases, suggesting higher call complexity.
* **Survey Scores vs Disconnect Type:** Managed disconnects score higher; technical failures result in lower satisfaction.
* **Hold Time vs Disconnect Type:** Certain disconnect types are associated with longer hold times, indicating operational inefficiencies.

Interpretations focus on **business impact and customer experience implications**.

---

##  Section E – Logical Reasoning

### **Question 18: Shape Grouping**

Shapes were grouped based on:

* Shape type (circles, polygons, quadrilaterals)
* Fill pattern (solid, striped, dotted, hollow)

All valid groupings were identified and clearly justified.

---

##  Tools & Technologies Used

* **Python:** Pandas, NumPy, Statsmodels, Matplotlib
* **SQL:** Aggregations, window functions, filtering
* **Database Tool:** DBeaver
* **Version Control:** Git & GitHub

---





---

