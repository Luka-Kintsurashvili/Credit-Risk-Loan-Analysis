# 📊 Retail Banking: Credit Risk & Portfolio Analytics Dashboard

## 📌 Project Overview
This project simulates a real-world banking credit-scoring process. Using a dataset of over 600 loan applications, I developed an end-to-end data pipeline to assess applicant risk, calculate debt stress, and visualize portfolio health.

The goal was to move beyond simple data entry and apply **Conservative Risk Modeling** to identify high-risk segments before loan approval.

---

## 🛠️ Tech Stack & Methodology
* **Tool:** Microsoft Excel (Advanced)
* **Engine:** Power Query (M) for ETL (Extract, Transform, Load)
* **Analytics:** Feature Engineering & Pivot Reporting
* **Foundational Knowledge:** ISET (Quantitative Economics) + Self-Directed Learning

---

## 🚀 Key Features & Workflow

### 1. Advanced ETL & Data Integrity
* **Handling Nulls:** Instead of simple deletion, I applied a "Banker's Choice" strategy. For categorical data, missing values were marked as `Unknown`.
* **Risk-Averse Imputation:** Missing values in the `Credit_History` column were treated as **0 (High Risk)**. This ensures the model doesn't underestimate potential defaults.

### 2. Financial Feature Engineering
I created custom metrics to mirror those used by institutions like the **Bank of Georgia (BOG)**:
* **Total Household Income:** Combined applicant and co-applicant incomes to assess true repayment capacity.
* **DTI (Debt-to-Income) Ratio:** Calculated the monthly loan burden relative to total income. 
* **Risk Segmentation:** Automated the categorization of applicants into `Critical Risk`, `High Debt Burden`, and `Standard` buckets based on credit history and a 40% DTI threshold.

### 3. Interactive Dashboard
The final dashboard features dynamic slicers that allow stakeholders to stress-test the portfolio across:
* **Education Level**
* **Property Area** (Urban/Semiurban/Rural)
* **Risk Segments** (Based on DTI and Credit History)

---

## 📈 Key Insights
* **Credit History is King:** Applicants with no credit history (0) faced a rejection rate of over 90%, regardless of their income level.
* **The 40% Threshold:** A significant portion of "Rejected" applications correlated with a DTI ratio exceeding 40%, validating the risk threshold used in the model.

---

## 📂 How to Use This Repo
1. **Download** the `.xlsx` file from this repository.
2. Open the file and navigate to the **Dashboard** sheet.
3. Use the **Slicers** on the left to filter the data.
4. Open **Power Query Editor** to see the "Applied Steps" for the data cleaning logic.

---
**About the Author:** I am a first-year undergraduate at the **International School of Economics (ISET)**. This project bridges the gap between economic theory and practical data engineering.
