# Humberto_Portfolio
Examples of Data Science Projects

# [Project 1: Customer Churn Analytics: Behavioral Profiling & Predictive Modeling](https://github.com/whitelotus2218/Humberto_Portfolio)

* **Tech Stack & Pipeline:**
  * SQL Server ──> Excel (`.xlsx`) ──> Python (Scikit-Learn) ──> Power BI
  * *(Cleaning ──> Storage ──> Lasso, RF & LogReg ──> Dashboards)*
* **Data Cleaning & EDA (SQL Server):**
  * Handled missing values, data types, and initial exploration using SQL Server Management Studio.
* **Preprocessing (Python):**
  * Applied Label Encoding, feature scaling, and feature selection via Lasso Regularization to isolate key drivers of churn.
* **Machine Learning:**
  * Trained a baseline Logistic Regression model.
  * Optimized Random Forest using `RandomizedSearchCV`.
  * Evaluated models using ROC-AUC and classification reports.
   <table>
  <tr>
    <td align="center">
      <img src="https://github.com/whitelotus2218/Humberto_Portfolio/blob/main/images/LassoChurn.png" width="200" alt="Model Comparison">
      <br>
      <sub><b>Lasso Analysis</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/whitelotus2218/Humberto_Portfolio/blob/main/images/Metric1.png" width="200" alt="ROC Curves">
      <br>
      <sub><b>RF and LR scores</b></sub>
    </td>
   <td align="center">
      <img src="https://github.com/whitelotus2218/Humberto_Portfolio/blob/main/images/Metric2.png" width="200" alt="ROC Curves">
      <br>
      <sub><b>RF and LR ROC curves</b></sub>
    </td>
  </tr>
</table>
  
* **Business Intelligence (Power BI):**
  * **Customer Profile Report:**
    * Behavioral segmentation and demographic overview.
  * **Churn Executive Dashboard:**
    * Churn rates and risk factor analysis.
  <table>
  <tr>
    <td align="center">
      <img src="https://github.com/whitelotus2218/Humberto_Portfolio/blob/main/images/churn_report1.png" width="400" alt="Model Comparison">
      <br>
      <sub><b>Model Comparison</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/whitelotus2218/Humberto_Portfolio/blob/main/images/churn_report2.png" width="400" alt="ROC Curves">
      <br>
      <sub><b>ROC Curves</b></sub>
    </td>
  </tr>
</table>
  

