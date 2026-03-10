Problem
- Exploratory analysis of over 3M taxi trips revealed that surcharges were applied inconsistently, with more than 70% concentrated in Manhattan during weekday business hours. This uneven distribution raised fairness concerns across zones and created operational ambiguity, as the underlying rules governing surcharge application were not clearly defined.

Action
1. -Driven Policy Analysis:
Developed classification models (Logistic Regression and Random Forest) to identify surcharge triggers across 3M+ trips, achieving ROC-AUC of 0.91. Applied SHAP analysis to interpret model outputs and uncover implicit policy patterns, confirming that pickup time and location were the dominant drivers.

2. Revenue & Equity Modeling:
Built Ridge Regression models to estimate the financial and distributional impact of surcharge policies, establishing a quantitative foundation for evaluating policy alternatives.

3. Strategic Scenario Simulation:
Designed and executed simulations for alternative surcharge policies (e.g., peak-hour or zone-based adjustments), comparing outcomes across revenue generation and equity metrics to identify more balanced strategies.

4. Reusable Framework Development:
Engineered a modular Python framework to support urban mobility policy experimentation, including components for policy definition, impact simulation, and evaluation of revenue and equity outcomes, enabling rapid testing of different policy scenarios.

<img width="858" height="952" alt="image" src="https://github.com/user-attachments/assets/d32d0e31-fcde-44bb-8767-2700cf018479" />


Results
1. Revenue Growth:
Generated a +0.9% increase in total revenue through optimized, data-driven time and zone-based pricing strategies.

2. Improved Policy Equity:
Reduced surcharge concentration in the three most affected zones by 22%, promoting a more balanced distribution of costs across the city.

3. Operational Transparency:
Delivered interpretable SHAP insights that clarified complex surcharge drivers, supporting more informed cross-functional policy and operational decisions.

4. Scalable Strategic Framework:
Developed a reusable analytical framework that converts large-scale mobility data into actionable policy recommendations, laying the groundwork for broader smart city and urban mobility initiatives.


<img width="590" height="390" alt="image" src="https://github.com/user-attachments/assets/2ff2e6d6-437d-4707-80e2-27de2bec5867" />


Tech Stack
To evaluate and improve NYC’s uniform congestion surcharge policy, this project designed and simulated an elastic fare system using large-scale data analysis and machine learning. Multiple modeling approaches—classification, regression, and clustering—were applied for different analytical objectives, with SHAP used to interpret model behavior. The analysis demonstrated that the proposed system could enhance both revenue performance and policy fairness.

Python

Data Engineering: pandas, numpy
Modeling: scikit-learn (classification, regression, clustering)
Model Interpretability (XAI): shap
Visualization: matplotlib, seaborn


