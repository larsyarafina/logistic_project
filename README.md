# 📦 US Logistics Performance Analysis with GenAI for Supply Chain Optimization
**📌 Project Overview**

**Objective:**\
This project analyzes the **US Logistics Performance Dataset** using a combination of **Data Analytics** and **Generative AI (IBM Granite models via Replicate API)**

The goal is to uncover insights into logistics operations, especially towards delay prediction and carrier optimization. GenAI will analyze the US Logistics Performance Dataset to create meaningful insights but also proposing actionable recommendations to improve logistics performance.

By combining **basic data analysis** (Python, Pandas, Matplotlib) with **GenAI-based reasoning**, this project provides both quantitative metrics and qualitative business insights.


## 📂 Raw Dataset
Dataset source: [US Logistics Performance Dataset – Kaggle](https://www.kaggle.com/datasets/shahriarkabir/us-logistics-performance-dataset)

**Background**\
Logistics directly impacts the efficiency of operational costs and competitiveness. By analyzing this dataset, companies and policymakers can identify performance bottlenecks, optimize routes, and invest in infrastructure more effectively.

The dataset includes shipment details such as:
- **Shipment_ID**
- **Origin Warehouse**
- **Destination**
- **Carrier**
- **Shipment & Delivery Dates**
- **Weight (kg)**
- **Cost**
- **Status**
- **Distance (miles)**
- **Transit Days**

## 🔍 Insights & Findings

### 1️⃣ Predict Delivery Delays (using status, dates, distance)
- **Factors:** Long distances, specific carriers, and seasonal shipment volumes contribute to higher delays.  
- **Trend:** Deliveries beyond ~1,500 miles show significantly higher late delivery probability.  
- **Business Takeaway:** Monitor long-distance shipments closely, and add buffer days for customers.

---

### 2️⃣ Optimize Carrier Selection (cost vs transit time)
- **Comparison:** Some carriers offer low cost but high transit days, while others are faster but more expensive.  
- **Trend:** For short-haul routes, carrier **A** is cost-efficient; for long-haul, carrier **B** balances speed & cost.  
- **Business Takeaway:** Use a **hybrid carrier strategy** based on route distance to reduce costs without impacting delivery speed.

---

### 3️⃣ Detect Anomalies (weights vs costs)
- **Outliers:** A few shipments show unusually high costs per kg, possibly due to fuel surcharges or data entry errors.  
- **Trend:** Most shipments follow a linear weight–cost relationship, but anomalies stand out in high-weight, low-cost ranges.  
- **Business Takeaway:** Investigate flagged shipments for potential billing or operational errors.

---

### 4️⃣ Forecast Shipping Expenses (by route)
- **Trend:** Expenses for some high-demand routes (e.g., East Coast to Midwest) are increasing steadily.  
- **Forecast:** Costs expected to rise **5–8% in the next quarter** on busiest lanes.  
- **Business Takeaway:** Renegotiate contracts or consider alternate carriers for cost-intensive routes.

---

## 🤖 AI Support Explanation
This project leverages **IBM Granite LLMs** (via Replicate API) to enhance analysis. Role of AI:
  - Interprets raw dataset samples and generates business-level insights.  
  - Explains trends, factors, and possible operational causes.  
  - Suggests recommended visuals (e.g., scatter plots, boxplots, time-series) to support findings.  

The manual analytics are most likely only gives numbers & plots, but AI can transforms them into **actionable business insights**, bridging the gap between data science and decision-making.

---

## 🚀 Tech Stack
- **Python (Pandas, Matplotlib, Seaborn)** – Data cleaning & visualization  
- **Replicate API** – Access IBM Granite GenAI models  
- **Google Colab** – Development environment  

---
