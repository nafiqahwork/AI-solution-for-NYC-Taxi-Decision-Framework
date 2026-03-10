## NYC Taxi Congestion Surcharge Optimization

---

## Project Overview
To evaluate and improve NYC’s uniform congestion surcharge policy, this project designs and simulates an elastic fare system using large-scale data analysis and machine learning. By applying multiple modeling approaches—classification, regression, and clustering—and interpreting results with SHAP, the project demonstrates how a redesigned pricing structure can improve both profitability and policy fairness.

---

## Problem
Exploratory analysis of 3M+ taxi trips revealed that congestion surcharges were applied inconsistently. 
- 70%+ of surcharges were concentrated in Manhattan
- Mostly occurred during weekday business hours
- Created fairness concerns across taxi zones
- Generated operational ambiguity, as the actual surcharge triggers were unclear
This indicated that the de-facto surcharge system differed from the intended policy rules.

---

## Methodology

1. Data-Driven Policy Analysis
- Built classification models (Logistic Regression, Random Forest) to identify surcharge triggers.
- Trained on 3M+ taxi trip records.
- Achieved ROC-AUC: 0.91.
- Applied SHAP for explainability.

Key Insight:
Pickup time and location were the strongest drivers of surcharge application.

2. Revenue & Equity Modeling
- Implemented Ridge Regression models to estimate:
  - Revenue impact
  - Distributional fairness
- Provided a quantitative baseline for evaluating policy alternatives.

3. Strategic Scenario Simulation
- Designed simulations to test alternative policies:
  - Peak-hour pricing adjustments
  - Zone-based exceptions
  - Hybrid congestion strategies

- Each scenario was evaluated using:
  - Revenue performance
  - Equity distribution across zones

4. Reusable Policy Simulation Framework
- Developed a modular Python framework enabling rapid policy experimentation.

- Framework modules:
  - Policy definition
  - Impact simulation
  - Revenue evaluation
  - Equity analysis

This allows analysts to test multiple urban mobility pricing strategies efficiently.

---

Analysis Visualization

<p align="center"> <img src="https://github.com/user-attachments/assets/d32d0e31-fcde-44bb-8767-2700cf018479" width="700"> </p>
<p align="center"> Figure 01: SHAP Feature Importance for Surcharge Prediction (Classifier Model) </p>

---

## Results: 

1. Revenue Growth
Optimized pricing increased total revenue by +0.9%.

2. Improved Policy Equity
Reduced surcharge concentration in the top 3 most affected zones by 22%, improving cost distribution across the city.

3. Operational Transparency
SHAP insights clarified complex surcharge triggers, enabling better cross-functional decision making.

4. Scalable Policy Tool
Delivered a reusable analytical framework capable of turning mobility data into actionable urban policy insights, supporting future smart-city initiatives.

---

<p align="center"> <img src="https://github.com/user-attachments/assets/2ff2e6d6-437d-4707-80e2-27de2bec5867" width="600"> </p>
<p align="center"> Figure 02: Modeled Revenue Trend: Before vs. After Optimization </p>
---

## Tech Stack

### Python

| Category | Tools |
|----------|------|
| Data Engineering | pandas, numpy |
| Modeling | scikit-learn (for Classification, Regression, Clustering)|
| Explainable AI | SHAP |
| Visualization | matplotlib, seaborn |

---

## Key Skills Demonstrated

- Machine Learning Modeling
- Explainable AI (XAI)
- Policy Simulation
- Urban Mobility Analytics
- Large Scale Data Analysis
- Revenue Optimization
