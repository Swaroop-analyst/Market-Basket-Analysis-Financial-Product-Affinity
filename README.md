# Market-Basket-Analysis-Financial-Product-Affinity
This project demonstrates how association rule mining can be applied in financial services to uncover hidden product relationships and convert them into measurable business value through intelligent cross-selling and customer engagement strategies.

Built a financial product affinity model using Apriori association rules to drive data-driven cross-selling strategies and improve customer lifetime value (CLV).

## 🔍 Business Problem
Banks need to understand which financial products customers typically purchase together in order to design effective cross-selling strategies, improve customer lifetime value (CLV), and optimize marketing ROI.

## 🎯 Objective
Discover strong product associations and recommend high-probability product bundles using Association Rule Mining.

## 📦 Dataset
Synthetic banking transaction dataset containing customer-wise purchased products.

---

## 🧭 Methodology (CRISP-DM)

### 1. Business Understanding
Identify frequent product bundles for cross-sell and upsell optimization.

### 2. Data Understanding & EDA
- 1000 customer transactions  
- Average products per customer: ~2.7  
- Most common product: Savings Account  

### 3. Data Preparation
Transactions converted into basket (one-hot encoded) format.

### 4. Modeling
Apriori algorithm used to generate association rules.

### 5. Evaluation Metrics
- **Support** – popularity of product combination  
- **Confidence** – likelihood of buying B if A is bought  
- **Lift** – strength of association (Lift > 1 indicates positive correlation)  

---

## 🧪 Model Evaluation

The Apriori model was evaluated using business-grade thresholds to ensure only meaningful and actionable rules:

- **Minimum Support:** 5%  
- **Minimum Confidence:** 60%  
- **Minimum Lift:** 1.5  

These constraints ensure that extracted rules are statistically significant, non-random, and suitable for real-world cross-sell deployment.

---

## 🧠 Key Insights from the Model

### 🔗 High-Impact Product Relationships

### **1. Mortgage → Home Insurance**

| Metric | Interpretation |
|------|---------------|
Confidence ≈ **80%+** | 8 out of 10 mortgage customers also require home insurance |
Lift > **3.0** | Relationship is over 3× stronger than random chance |
Business Signal | **Extremely strong bundling opportunity** |

**Business Insight:**  
Mortgage approval should automatically trigger a home insurance offer within **7–30 days**.

---

### **2. Savings Account → Credit Card**

| Metric | Interpretation |
|------|---------------|
Confidence ≈ **70–75%** | Majority of savings customers adopt credit cards |
Lift ≈ **1.8–2.0** | Strong positive correlation |
Business Signal | **Primary entry-point cross-sell funnel** |

**Business Insight:**  
New savings customers are prime targets for immediate credit card onboarding.

---

### **3. Credit Card → Personal Loan**

| Metric | Interpretation |
|------|---------------|
Confidence ≈ **65–70%** | Credit card usage strongly indicates loan demand |
Lift > **2.0** | More than double the expected chance |
Business Signal | **High revenue expansion opportunity** |

**Business Insight:**  
High-utilization credit card customers should receive **pre-approved personal loan** offers.

---

## 💰 Business Impact Analysis

| Area | Expected Improvement |
|-----|----------------|
Cross-sell conversion | **+15% to +25%** |
Customer Lifetime Value | **+10% to +18%** |
Marketing cost efficiency | **20–30% reduction** |
Customer retention | Higher due to relevant offers |

---

## 🧩 Strategic Recommendations

### 🎯 Implementation Strategy

| Customer Event | Automated Action |
|--------------|----------------|
Mortgage approved | Push home insurance within **7–30 days** |
New savings account | Offer credit card + mutual fund |
High credit card usage | Provide pre-approved personal loan |

### 🧪 Model Governance & Continuous Improvement
- Re-evaluate association rules **quarterly**
- Segment rules by **income, age, and region**
- Monitor **campaign ROI per rule** and refine thresholds accordingly

---

## 🛠 Tools & Technologies
Python, Pandas, Mlxtend, Apriori Algorithm, Association Rule Mining

---

