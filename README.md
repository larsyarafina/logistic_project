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
- **Factors:** Long distances, specific carriers, and seasonal shipment volumes contribute to higher delivery delays.  
- **Trend:** Deliveries beyond ~1,500 miles show significantly higher the probability of late delivery.  
- **Business Takeaway:** Monitor long-distance shipments closely, evaluate carrier performance, and increace both capacity and resources during peak seasons.

---

### 2️⃣ Optimize Carrier Selection (cost vs transit time)
- **Carrier ranking**: USPS and UPS for short-distances routes. DHL, USPS, Amazon Logistics for long-distances route.
- **Business Conclusion**: UPS is the cheapest and fastest carrier for short-distance routes. FedEx offering competitive costs and transit times for both short and long routes.
- **Summary**:  The dataset analysis reveals that UPS is the most cost-effective carrier for short-distance shipments, while FedEx stands out for both speed and balanced performance across both short and long routes. DHL and Amazon Logistics are competitive for long-distance shipments, though they tend to be more expensive. LaserShip and USPS are also viable options, particularly for long-distance routes, but generally come with higher costs.

---

## 🤖 AI Support Explanation
This project leverages **IBM Granite LLMs** (via Replicate API) to enhance analysis. Role of AI:
  - Interprets raw dataset samples into clear narratives.
  - Generates structured insights by connecting metrics with operational meaning.
  - Suggests comparisons and conclusions that go beyond raw statistics.


While traditional analytics can shows what the numbers are (delays, cost, anomalies), Generative AI is able to explains why it matters for the business and what to do next. Therefore, GenAi is able to provides human-like recommendation for logistics optimization.

---

## 🚀 Tech Stack
- **Python (Pandas, Matplotlib, Seaborn)** – Data cleaning & visualization  
- **Replicate API** – Access IBM Granite Instruct GenAI models  
- **Google Colab** – Development environment  

---
