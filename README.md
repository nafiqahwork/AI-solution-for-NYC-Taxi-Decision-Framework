<img width="858" height="952" alt="image" src="https://github.com/user-attachments/assets/d32d0e31-fcde-44bb-8767-2700cf018479" />Problem
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







