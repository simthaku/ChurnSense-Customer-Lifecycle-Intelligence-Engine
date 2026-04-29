# 🧠 ChurnSense  
### Customer Lifecycle Intelligence & Experience Orchestration Engine

> “Not just predicting churn — orchestrating decisions across the customer lifecycle.”

---

## ⚡ Problem Context

In subscription-driven businesses, churn is not a one-time event.  
It is the result of progressive customer disengagement across lifecycle stages.

Most solutions:
- Detect churn too late  
- Focus only on reporting  
- Lack actionable outputs  

---

## 🎯 What I Built

An end-to-end customer intelligence system that transforms raw data into decisions.

Raw Customer Data → Predictive Signals → Business Actions


---

## 🧩 System Architecture

<pre>
Customer Data (Raw)
↓
SQL ETL Layer (Staging → Clean → Views)
↓
Analytical Layer (Segmentation + KPIs)
↓
Power BI Dashboard (Business View)
↓
Machine Learning Model
↓
Prediction Output (At-Risk Customers)
↓
Action Layer (Retention Targeting)
</pre>


---

## 🔍 Key Capabilities

### 1️⃣ Behavioral Intelligence (SQL + EDA)
- Customer segmentation by:
  - Contract type  
  - Tenure  
  - Revenue  
  - Services  
- Identified early churn patterns  

---

### 2️⃣ Business Dashboard (Power BI)
- Executive KPIs:
  - Total Customers  
  - Churn Rate  
  - Revenue  
- Interactive filters for deep analysis  
- Segment-level churn insights  

---

### 3️⃣ Predictive Intelligence (ML)
- Model: Random Forest  
- Objective: Predict future churn  

Clean Data → Encode → Train → Evaluate → Predict


- Output:
  - Customer-level churn prediction  
  - Binary classification (0 / 1)

---

### 4️⃣ Decision Layer
- Converted predictions into:
  - High-risk customer list  
  - Business-ready dataset  
- Enables proactive retention actions  

---

## 📊 Dashboard Insights (Power BI)

### 🔹 Churn Analysis Dashboard

![Churn Analysis](Churn_analysis_summary.png)

This dashboard provides a comprehensive view of customer churn:

- KPIs Overview:
  - Total Customers: 6,418  
  - Total Churn: 1,732  
  - Churn Rate: 27%  
  - New Joiners: 411  

- Key Drivers:
  - Month-to-month contracts show highest churn  
  - Low tenure customers are more vulnerable  
  - Higher monthly charges increase churn risk  

- Business Value:
  - Identifies high-risk segments  
  - Supports retention strategy planning  

---

### 🔹 Churn Prediction Dashboard

![Churn Prediction](Churn_analysis_prediction.png)

This dashboard operationalizes machine learning predictions:

- Displays predicted churn customers  
- Provides customer-level profiling  
- Enables:
  - Targeted retention campaigns  
  - Personalized offers  

- Business Value:
  - Converts predictions into actionable insights  
  - Bridges analytics with decision-making  

---

## 📈 Key Business Insights

### 1. Overall churn rate is 27% — 1 in 4 customers is leaving
Out of 6,418 total customers, **1,732 have churned**. With 411 new joiners not yet contributing meaningful revenue, retention of existing customers is the top priority.

### 2. Month-to-month contracts are the biggest churn driver
Contract type churn rates: **Month-to-Month: 46.5%** vs One Year: 11.0%. Nearly half of all flexible-contract customers churn — a clear signal that long-term contract incentives could significantly reduce attrition.

### 3. Fiber Optic users churn at 41.1% — the highest among internet types
Despite Fiber Optic being the premium service, it has the highest churn rate (41.1%), compared to Cable (25.7%) and DSL (19.4%). This points to a service quality or pricing perception problem for high-paying customers.

### 4. Older customers churn most — 31% churn rate in the 50+ age group
Churn rate climbs with age: `<20: low`, `20-35: 23.5%`, `35-50: 24%`, `>50: 31%`. Senior customers may need targeted support or simpler service plans.

### 5. Jammu & Kashmir has the highest state-level churn at 57.2%
Geographic churn is highly concentrated — Jammu & Kashmir (57.2%), Assam (38.1%), and Jharkhand (34.5%) are significantly above the national average. Regional service or pricing issues may be driving this.

### 6. Competitor activity is the #1 churn reason (761 customers)
The churn category breakdown shows: Competitor (761) > Attitude (301) > Dissatisfaction (300) > Price (196). Competitive pricing and feature comparison should be the focus of retention strategy.

### 7. Internet Service is used by 80.5% of churned customers
The services table shows Internet_Service has 80.50% adoption among churned customers — the highest of any service. Customers with internet are more likely to compare providers and switch.

### 8. ML model identified 376 new joiners already at risk
The Random Forest model scored all new joiners and flagged **376 customers as predicted churners** before they actually churn — enabling proactive outreach while there's still time to retain them.

---

## 📊 Model Performance

- Accuracy: ~80%  
- Metrics:
  - Precision  
  - Recall  
  - F1 Score  
  - Confusion Matrix  

---

## 🛠️ Tech Stack

| Layer | Tool |
|---|---|
| Database & SQL | MySQL |
| Data Cleaning | SQL (ISNULL, CASE, staging → prod pipeline) |
| Visualization | Power BI Desktop (2-page dashboard) |
| Data Transformation | Power Query (M language) |
| DAX Measures | Power BI DAX |
| ML Model | Python — scikit-learn Random Forest |
| ML Environment | Jupyter Notebook (Anaconda) |

---

## 🧪 Engineering Decisions

- Maintained training vs prediction consistency  
- Handled unseen categories in new data  
- Avoided data leakage (excluded churn reason fields)  
- Built reusable SQL views for BI + ML  

---

## 🚀 Business Impact

- Early churn detection  
- Targeted retention strategies  
- Improved revenue stability  
- Better decision-making  

---

### Customer Lifecycle Segmentation

New → Active → At Risk → Churned



### Action Recommendation Layer

At Risk → Retain
High Value → Upsell
Stable → Monitor

## 🧠 My Approach
Data → System → Decision → Impact


---

## 🎯 Key Takeaway

This is not:
- A churn dashboard  
- A standalone ML model  

This is:
- A customer intelligence system  
- A decision-support engine  

---

## 💡 What This Project Demonstrates

- ✅ End-to-end analytics pipeline: SQL → Power BI → Python ML
- ✅ Production-quality SQL data cleaning with business-driven null handling
- ✅ Creating SQL views to cleanly separate analytical and prediction datasets
- ✅ Power Query transformations: computed columns, mapping tables, column unpivoting
- ✅ DAX measure writing for dynamic KPI cards
- ✅ Random Forest classification with proper train/test split and label encoding
- ✅ Preventing data leakage by reusing training encoders on new data
- ✅ Closing the loop — bringing ML predictions back into Power BI for business consumption

---

## ⭐ If You Like This Project

- Star ⭐ the repo  
- Let’s connect and discuss data  



