#  Credit Risk Analysis: End-to-End Data Pipeline

###  Project Overview
This project demonstrates a complete data science workflow, transforming raw banking data into actionable financial insights. The pipeline moves from initial data cleaning and modeling in **Python**, to structured storage in **SQLite**, and finally to an interactive executive dashboard in **Power BI**.

The analysis focuses on a portfolio of **30,000 customers** to predict default probabilities and identify high-risk segments for a banking institution.

---

###  The Technical Pipeline

1.  **Data Processing (Python/Jupyter):**
    * Cleaned the raw UCI Credit Card dataset and performed feature engineering.
    * Developed a model to calculate **Predicted Risk Probabilities**.
    * *Tools: Pandas, Matplotlib, Scikit-learn, Pickle.*

2.  **Database Management (SQL):**
    * Migrated the cleaned dataset into a **SQLite** database (`Bank_Credit_Risk.db`).
    * Structured the data to support relational reporting and efficient querying.
    * *Tools: SQLite, SQL Subqueries.*

3.  **Data Visualization (Power BI):**
    * Connected Power BI to the SQLite database for real-time reporting.
    * Developed dynamic DAX measures for **Risk Tiers** and **Portfolio Exposure**.
    * Created a specialized **Risk Distribution Histogram** to visualize the bimodal nature of the model's predictions.
    * *Tools: Power BI, DAX, Power Query.*

---

###  Key Business Insights
* **Portfolio Health:** The average risk probability across the portfolio is **40.02%**.
* **Bimodal Risk Distribution:** Identified a specific high-risk cluster at the **85-90%** probability range, allowing for targeted credit tightening.
* **Demographic Trends:** The "Over 60" age group holds the highest average credit limit (**$202K**), highlighting a high-exposure segment for the bank.
* **Interactive Filtering:** Education and Age slicers allow for granular analysis of how demographics impact the bank's total exposure.

---

###  Repository Structure
* `Data/`: Contains the raw CSV, cleaned data, and the SQLite database file.
* `Notebooks/`: Includes the Jupyter Notebook with the Python logic and the `.pkl` model.
* `Dashboard/`: The final `.pbix` Power BI project file.

---

###  How to Use
1.  **Python:** View `credit_card_project.ipynb` to see the data cleaning and modeling logic.
2.  **SQL:** The `Bank_Credit_Risk.db` file can be explored using any SQL editor (e.g., DBeaver or SQLite Browser).
3.  **Power BI:** Open `Credit_Risk_Dashboard_V1.pbix`. 
    * *Note: If the data doesn't load, update the Data Source settings in Power BI to point to the local path of the `.db` file on your machine.*

---

