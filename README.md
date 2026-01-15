# 📊 Credit Risk Analytics & Client Segmentation  
**Consulting Competition Winning Project**

---

## 🏆 Overview

This project was developed as part of a **credit risk analytics consulting competition**, where our team analyzed large-scale client credit data to improve **risk assessment, client segmentation, and future credit extension strategies**.

The project combined **data cleaning, statistical modeling, and business-driven visualization** to deliver actionable recommendations for financial institutions. I **led a team of 4**, guided the analytical direction, and translated insights into **executive-ready recommendations**. The project was selected as the **winning solution** in the competition.

---

## 🎯 Problem Statement

Financial institutions face increasing pressure to:

- Accurately distinguish **low-risk vs high-risk clients**
- Reduce **non-performing loans**
- Optimize **client targeting and portfolio growth**

The challenge was to use historical application and credit data to:

- Understand what differentiates **good and bad clients**
- Evaluate predictive models for **credit risk**
- Recommend **data-driven credit extension and risk mitigation strategies**

---

## 🗂 Dataset Overview

- **Total records:** 36,000+ unique clients  
- **Data sources:**
  - `application_record` (demographics & financial attributes)
  - `credit_record` (monthly payment history)

### Key Variable Groups

- **Demographics:** Age, gender, family size, marital status  
- **Employment & Income:** Income type, annual income, occupation, employment duration  
- **Housing & Assets:** Property ownership, housing type, car ownership  
- **Credit Behavior:** Repayment patterns, overdue status, client classification (Good/Bad)

---

## 🧹 Data Cleaning & Preprocessing

Key preprocessing steps included:

- Removal of variables with **low sampling adequacy** (Chi-Square & KMO tests)
- Handling **multicollinearity** through correlation analysis
- Dummy encoding of categorical variables (e.g., income type)
- Standardization and numeric conversion for modeling compatibility

These steps ensured the dataset was **statistically robust and modeling-ready**.

---

## 📈 Analytical Approach

### 1. Exploratory Data Analysis (EDA)

Conducted using **Tableau**, focusing on:

- Income distribution and outliers
- Client segmentation by education, employment, and income
- Credit repayment behavior across risk groups

<p align="center">
  <img src="images/correlation heatmap.png" width="600">
</p>

**Example Insight:**  
Pensioners and state servants showed **high repayment reliability**, while working clients dominated portfolio volume but exhibited **varied risk behavior**.

<p align="center">
  <img src="images/client_distribution_income.png" width="600">
</p>

---

### 2. Statistical & Predictive Modeling

The following models were evaluated:

| Model               | Purpose                          | Accuracy        |
|--------------------|----------------------------------|-----------------|
| Logistic Regression | Binary credit classification     | 42.07%          |
| Naïve Bayes         | Probabilistic risk estimation    | Context-dependent |
| Decision Tree       | Rule-based interpretability      | **84.94%**      |

- **SMOTE** was applied to address class imbalance
- Decision trees provided the highest accuracy but revealed bias toward majority classes
- Logistic regression offered interpretable predictors such as **income, age, and employment duration**

<p align="center">
  <img src="images/Decision Tree Model.png" width="700">
</p>

---

## 🔍 Key Insights

### Insight 1: Income Type Matters
- Working clients form the majority but show mixed repayment behavior
- Pensioners and State Servants consistently demonstrate low credit risk
- Commercial associates exhibit comparatively higher default rates

<p align="center">
  <img src="images/Income Insight.png" width="650">
</p>

<p align="center">
  <img src="images/Income Insight 2.png" width="650">
</p>
---

### Insight 2: Education Correlates with Creditworthiness
- Academic degree holders show:
  - Highest average income
  - ~90% good-client ratio
- Secondary education dominates portfolio volume but shows higher variability

<p align="center">
  <img src="images/Education Insight.png" width="650">
</p>
---

### Insight 3: Repayment Behavior Is a Strong Risk Signal
- **Good clients** cluster around:
  - Paid Off
  - 1–29 Days Overdue
- **Bad clients** concentrate in:
  - 90+ Days Overdue
  - Repeated inactive or no-loan statuses

<p align="center">
  <img src="images/Repayment Behaviour.png" width="650">
</p>

---

## 💡 Business Recommendations

### ✅ Risk Mitigation
- Proactively monitor early delinquency buckets (1–29, 30–59 days overdue)
- Introduce early-warning systems and payment nudges
- Apply restructuring or settlement strategies for chronic defaulters

---

### 🎯 Client Segmentation & Growth
- Expand offerings for **low-risk segments** (Pensioners, State Servants)
- Design premium products for **high-income & academic degree holders**
- Introduce tailored **student credit products** to grow underrepresented segments

---

### 📊 Model Improvements
- Incorporate additional features (housing stability, education)
- Explore cost-sensitive learning or ensemble models
- Continue addressing class imbalance to improve minority class prediction

---

## 🧠 My Role & Leadership

- Led a **4-member consulting team**
- Drove analytical direction and model selection
- Translated technical results into **executive-level insights**
- Designed and presented the **final client-ready narrative**
- Coordinated **report writing and presentation delivery**

---
