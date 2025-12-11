---
title: "OM 621 Analytics Portfolio"
author: "Natasha Christina Sulistyo"
course: "OM 621 — Tools & Technologies for Analytics"
semester: "Fall 2025"
description: "A comprehensive analytics portfolio featuring Python exploratory analysis, transportation delay insights, invoice time-series evaluation, and cost forecasting foundations. Includes Assignment 1 storytelling framework, Assignment 2 EDA, Assignment 3 delay/time-series analysis, and supporting visual outputs."
layout: page
nav_order: 1
---

# 🧠 OM 621 Analytics Portfolio  
**Author:** Natasha Christina Sulistyo  
**Course:** OM 621 — Tools & Technologies for Analytics  
**Semester:** Fall 2025  

---

# 🎥 Video Overview (3–5 Minutes)

<iframe src="https://drive.google.com/file/d/1-X7hjIxO86yzcB3tOUyDtnnXDm-EfONQ/preview" 
width="850" height="480" allow="autoplay"></iframe>

---

# 📌 Project Overview

This repository contains the full analytical workflow completed for OM 621 across three assignments:

- **Assignment 1 — Business storytelling and storyboard design**  
- **Assignment 2 — Python data expectations and exploratory analysis**  
- **Assignment 3 — Python-based delay distribution, time-series behavior, and cost forecasting insights**  

These deliverables collectively demonstrate data understanding, exploratory analytics, transportation delay evaluation, operational insight generation, and professional storytelling.

---

# 🟦 Assignment 1 — Context, Audience, Storytelling, and Storyboard  
**Based on:** Assignment 1 Submission

Assignment 1 establishes the narrative and strategic foundation for the analytics project. It defines the *Who, What, and How*, analyzes audience needs, identifies required data, and delivers a full 3-minute story and conceptual storyboard.

---

## 🔹 1. Who, What, and How

### **Who — Audience**
The target audience is the **Director of Supply Chain at Qualcomm**.  
As an external analytics expert previously engaged in logistics optimization, you and the director share aligned goals in:

- Cost management  
- Operational visibility  
- Data-driven decision-making  

---

### **What — Recommendation**
I propose the adoption of a **predictive analytics system** to:

- Forecast transportation costs  
- Improve budgeting accuracy  
- Allocate divisional expenses more effectively  
- Reduce surprises caused by late or inconsistent invoicing  

This highlights the business stakes and motivates decision-makers.

---

### **How — Presentation Strategy**
Approach uses:

- Historical shipment and invoice data  
- Predictive models to estimate upcoming transportation costs  
- A **live, interactive dashboard** featuring:
  - Time-series visuals  
  - Slope charts  
  - Division-level breakdowns  
  - Operational insights  

Live presentation ensures clarity and control during explanation.

---

## 🔹 2. Understanding the Audience

To better tailor analytics communication to the Director of Supply Chain, the following steps were identified:

1. **Research background & priorities**  
   Review LinkedIn, supply-chain reports, and Qualcomm performance metrics.

2. **Direct conversation**  
   Discuss pain points such as late invoices and budgeting volatility.

3. **Operational document review**  
   Explore internal benchmarks, division interactions, and variance root causes.

These insights shape the tone, emphasis, and design of the final dashboard and analysis.

---

## 🔹 3. Data Needs

To build an effective cost-forecasting analytics solution, the following features and breakdowns are required:

### **Key Variables**
- Shipment date  
- Carrier  
- Origin & destination  
- Mode (air, ship, truck)  
- Weight or volume  
- Invoice amount  
- Invoice date  
- Division / business unit  
- Shipment type (parcel/container)

### **Essential Breakdowns**
- **By division** → cost allocation  
- **By mode/carrier** → performance differences  
- **By month/quarter** → forecasting granularity  
- **Historical vs predicted** → validation and accuracy  

Visualizations include line charts, clustered bar charts, scatterplots, and slope charts (avoid pie charts for comparisons).

---

## 🔹 4. 3-Minute Story

> “Imagine trying to manage your quarterly budget while invoices for global chip shipments arrive weeks or months late. Qualcomm’s divisions move products worldwide using multiple carriers, and unpredictable billing cycles create cost overruns and financial stress.  
> 
> But what if we could predict these transportation costs ahead of time? Using Qualcomm’s historical shipment data, we can build a forecasting system that alerts you to rising trends and helps divisions allocate budgets accurately.  
> 
> Picture a dashboard that clearly shows estimated vs. actual costs, slopes illustrating direction of change, and early warnings when costs deviate. With this system, Qualcomm can reduce budgeting errors by 20–30%, improve cash flow, and create accountability across divisions. This is how we move from uncertainty to control.”

---

## 🔹 5. Storyboard Summary

My storyboard includes five conceptual stages:

1. **Problem framing** — Budget unpredictability from late invoices  
2. **Data reality** — Operational lags, trends in shipments and costs  
3. **Predictive modeling** — Cost estimation & trend forecasting  
4. **Dashboard walkthrough** — Interactive visuals for divisional planning  
5. **Call to action** — Implement forecasting system → gain control  

---

## 🔹 6. Envisioned Successful Solution

A successful analytics solution includes:

- ERP-integrated predictive cost dashboard  
- 85%+ forecasting accuracy  
- Alerts for anomalies and cost overruns  
- Effective visuals aligned with perception best practices  
- Monthly & quarterly forecast generation  
- Improved divisional budgeting and transparency  

---

# 🟦 Assignment 2 — Python Data Expectations & Exploratory Analysis  
**Notebook:** [assignment_2.ipynb](notebooks/assignment_2.ipynb)

Assignment 2 focuses on understanding data expectations, validating initial assumptions, and performing foundational exploratory analysis on the transportation dataset.

---

## 🔹 1. Data Expectations Review  
This section compares early expectations from Assignment 1 to the reality of the dataset.

Key insights include:

- Certain fields (such as invoice date and invoice amount) contain meaningful missing values.  
- Missingness reflects real operational processes, such as shipments recorded before invoices are issued.  
- Data quality issues highlight workflow delays and asynchronous operational timing.  

This ensures correctness in assumptions before deeper analytical work.

---

## 🔹 2. Basic Exploration  
The notebook performs structural and statistical exploration, including:

- Counting non-null values across all columns  
- Identifying attributes with the most missing entries  
- Computing summary statistics (mean, min, max invoice amounts)  
- Observing operational reasons behind missing invoices  

This step builds the analytical foundation for later assignments.

---

## 🔹 3. Interpretation of Missingness  
Assignment 2 emphasizes understanding the *meaning* of missing data.

Key interpretations:

- Invoice dates missing because billing has not yet occurred  
- Shipment activity often precedes financial posting  
- Some fields are complete due to standardized operational requirements  

---

## 🔹 4. Early Observations & Visuals  
Although forecasting is not performed yet, early patterns begin to emerge:

- Invoice amounts vary noticeably  
- Delays appear to differ across shipments  
- Potential seasonality and variability cues appear in the data  

---

## 🔹 5. Key Takeaways  
Assignment 2 establishes:

- A clear understanding of dataset structure  
- Recognition of meaningful operational gaps  
- Initial insights that support deeper analysis in Assignment 3  

---

# 🟦 Assignment 3 — Python Delay Analysis, Time-Series Behavior & Cost Forecasting Foundations  
**Notebook:** [assignment_3.ipynb](notebooks/assignment_3.ipynb)

Assignment 3 expands upon Assignment 2 with structured visual analytics and conceptual forecasting insights.

---

## 🔹 1. Delay Distribution by Mode  
A delay distribution plot was generated and exported as:

This section evaluates:

- Delay variability by transportation mode  
- Skewness and tail behavior  
- Mode-specific reliability patterns  

This allows operational teams to compare timeliness across shipping methods.

---

## 🔹 2. Invoice Time Series Analysis  
Time-series visualization explores:

- Mild upward trends in invoice amounts  
- Short-term volatility likely tied to batching or operational cycles  
- Potential seasonal rhythms  
- Variability relevant for forecasting  

All exported visualizations for this analysis can be found in the **plots** folder:  
➡️ [View Plots](plots/)


---

## 🔹 3. Cost Estimation & Forecasting Reflections  
The notebook provides conceptual forecasting insights including:

- Cost appears influenced by short-term operational events  
- A slight rising trend exists over the period  
- Forecasting must capture both noise and general direction  
- Mode-based cost behavior suggests different operational strategies  

This establishes the analytical logic for future modeling.

---

## 🔹 4. Visual Analytics Output  
Charts illustrate:

- Transportation delay patterns  
- Invoice behavior over time  
- Cost variability indicators  

These visuals prepare insights for integration into dashboards and presentations.

---

## 🔹 5. Conclusions  
Assignment 3 reveals:

- Transportation delays differ meaningfully by mode  
- Invoice amounts show upward tendencies with volatility  
- Operational workflows significantly influence data patterns  
- Insights support transportation planning and cost forecasting decisions  

---

# 📊 Power BI Dashboard  
**File:** [Assignment_4.pbix](pbi/Assignment_4.pbix)

The Power BI dashboard provides an interactive way to explore insights from both Python assignments.  
It includes:
- Delay summaries  
- Invoice time-series visuals  
- Transportation mode comparisons  
- KPI metrics  
- Clean and consistent layout design  


# 📁 Repository Structure

om621-assignments/
│
├── data/
│ └── tr_data_22_24.csv
│
├── notebooks/
│ ├── assignment_2.ipynb
│ └── assignment_3.ipynb
│
├── plots/
│ ├── delay_dist_by_mode.png
│ └── invoice_timeseries.png
│
├── pbi/
│ └── assignment4.pbix
│
└── README.md


---

# 🏁 Final Reflection

This OM 621 portfolio demonstrates:

- Strong exploratory and analytical Python skills  
- Understanding of operational data structures  
- The ability to interpret delays, invoice timing, and cost behaviors  
- Professional communication of insights through visuals and structured storytelling  

Each assignment contributes to a complete, decision-ready analytics narrative.

---

# 🙌 Acknowledgment 
Thank you to Prof. Majid Karimi for guidance, support, and feedback throughout the course.

