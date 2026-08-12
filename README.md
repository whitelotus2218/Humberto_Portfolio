# Humberto_Portfolio
Examples of Data Science Projects

# Project 1: Customer Churn Analytics: Behavioral Profiling & Predictive Modeling

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
      <img src="https://github.com/whitelotus2218/Humberto_Portfolio/raw/main/images/LassoChurn.png" width="300" alt="Model Comparison">
      <br>
      <sub><b>Lasso Analysis</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/whitelotus2218/Humberto_Portfolio/raw/main/images/Metric1.png" width="300" alt="ROC Curves">
      <br>
      <sub><b>RF and LR scores</b></sub>
    </td>
   <td align="center">
      <img src="https://github.com/whitelotus2218/Humberto_Portfolio/raw/main/images/Metric2.png" width="300" alt="ROC Curves">
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
      <img src="https://github.com/whitelotus2218/Humberto_Portfolio/raw/main/images/churn_report1.png" width="400" alt="Model Comparison">
      <br>
      <sub><b>Model Comparison</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/whitelotus2218/Humberto_Portfolio/raw/main/images/churn_report2.png" width="400" alt="ROC Curves">
      <br>
      <sub><b>ROC Curves</b></sub>
    </td>
  </tr>
</table>

# Project 2: Customer Segmentation & Marketing Campaign Analytics (Unsupervised Learning)

* **Tech Stack & Pipeline:**
  * Python (Pandas, Scikit-Learn, Seaborn, Matplotlib)
  * *(Cleaning ──> Feature Engineering ──> Scaling ──> PCA ──> Clustering ──> Profiling)*
* **Data Cleaning & Preprocessing:**
  * Handled missing values and removed statistical outliers for age and income.
  * Applied Label Encoding to categorical attributes and normalized features using `StandardScaler`.
* **Feature Engineering:**
  * Created key behavioral metrics: Customer tenure (`Customer_For`), total spending (`Spent`), household structure (`Family_Size`, `Is_Parent`, `Living_With`), and consolidated education levels.
* **Dimensionality Reduction & Clustering:**
  * Implemented Principal Component Analysis (PCA) to reduce dimensionality into 3 principal components.
  * Used the Elbow Method (`KElbowVisualizer`) and applied **Agglomerative Clustering** (k=4) to segment customers into distinct behavioral groups.
 
 
 <table>
  <tr>
    <td align="center">
      <img src="https://github.com/whitelotus2218/Humberto_Portfolio/raw/main/images/ElbowAnalysis.png" width="400" alt="Model Comparison">
      <br>
      <sub><b>Elbow Analysis</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/whitelotus2218/Humberto_Portfolio/raw/main/images/ClusterResult.png" width="400" alt="ROC Curves">
      <br>
      <sub><b>Cluster visualization</b></sub>
    </td>
  </tr>
</table>

* **Business Insights & Campaign Analysis:**
  * **Customer Behavioral Profiling:**
    * Visualized cluster segments using income vs. spending scatter plots.
  * **Marketing Response Evaluation:**
    * Analyzed campaign acceptance rates (`Total_Promos`) across clusters to identify high-value target segments.

  <table>
  <tr>
    <td align="center">
      <img src="https://github.com/whitelotus2218/Humberto_Portfolio/raw/main/images/ClusterProfileSpend.png" width="400" alt="Model Comparison">
      <br>
      <sub><b>Cluster Spend Profile</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/whitelotus2218/Humberto_Portfolio/raw/main/images/ClusterPromotion.png " width="400" alt="ROC Curves">
      <br>
      <sub><b>Cluster classification by promotion feature</b></sub>
    </td>
  </tr>
</table>


# Project 3: Customer Shopping Behavior Analytics & SQL Data Warehouse

* **Tech Stack & Pipeline:**
  * Python (Pandas, SQLAlchemy), PostgreSQL, Power BI
  * *(Cleaning & Transformation ──> PostgreSQL Database ──> Power BI Dashboard)*
* **Data Cleaning & Preprocessing (Python):**
  * Handled missing values in customer review ratings by imputing category-specific medians (robust to outliers).
  * Standardized column names (lowercase and snake_case format) for better data querying.
  * Engineered a new numerical metric (`purchase_frequency_days`) by mapping text-based purchase intervals to exact days.
  * Verified data consistency (checked correlation between discounts and promo codes) and dropped redundant columns.
* **Database Integration (PostgreSQL):**
  * Established a secure database connection using SQLAlchemy (`psycopg2`).
  * Loaded the cleaned Pandas DataFrame directly into a PostgreSQL database table (`customer`), setting up the foundation for structured querying.
* **Business Intelligence (Power BI):**
  * Developed an interactive executive dashboard connected to the PostgreSQL warehouse to analyze shopping trends, purchasing frequency, and customer spending habits.
 ![](https://github.com/whitelotus2218/Humberto_Portfolio/raw/main/images/BISales.png)
