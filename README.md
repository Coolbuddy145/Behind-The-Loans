# 📊 Financial Loan EDA & Insights

## 🔎 Project Overview

This project explores a financial loans dataset to understand borrower behavior, loan disbursement patterns, and risk factors. The focus is on **exploratory data analysis (EDA)** and **business insights**, rather than predictive modeling. The analysis covers data cleaning, univariate and bivariate analysis, correlation checks, and business recommendations.

---

## ⚙️ Data Preparation

* **Dropped `emp_title`** due to large number of nulls and low predictive value (kept `emp_length` instead).
* **Converted `term`** from object (e.g., "60 months") to integer (60) for proper analysis.
* **Dropped `id`, `member_id`, and `total_acc`** as they have little analytical or predictive significance.
* **Outliers kept intentionally** since they represent real-world cases (e.g., high incomes, large loans, high payments). The focus here is insights, not ML model training.

---

## 📈 Key Insights

### 1. Loan Purpose

* **Most loans** are taken for **debt consolidation** and **credit card repayment**.
* Loan purposes such as **medical, education, and home improvement** are underrepresented.
* **Recommendation:** The bank could diversify by offering targeted loan products (e.g., education or medical loans) with competitive rates to grow in these segments.

### 2. Home Ownership

* Majority of borrowers are either **renters** or **mortgage holders**; very few own their homes outright.
* **Recommendation:** Create specialized loan products — home renovation loans for renters/mortgage holders, and investment/business loans for outright homeowners.

### 3. Loan Tenure

* Loans are offered in **two tenures: 36 and 60 months**.
* **36-month loans dominate**, indicating preference for shorter, lower-risk lending.

### 4. Borrower Profile

* Borrowers with **10+ years of work experience** receive the highest loan amounts, likely seen as low-risk due to stable employment.
* For borrowers with <10 years of experience, loan amounts don’t show a strong pattern with tenure.

### 5. Loan Amount & Interest Rate

* Scatter analysis shows **heavy clustering around smaller loans (<15,000)** with moderate interest rates (7–15%).
* No strong correlation between loan amount and interest rate.

### 6. Grade & Interest Rate

* Strong **positive correlation (0.94)** between **loan grade and interest rate**.
* Lower grades → higher rates; higher grades → lower rates.
* This confirms the **bank uses grading to set loan pricing.**

### 7. Grade & Default Risk

* Loan performance strongly aligns with grade:

  * **Grades A & B:** Lowest default rates (most loans fully paid).
  * **Grades C–E:** Rising charge-offs.
  * **Grades F & G:** High-risk, with significant defaults.
* Confirms the **grading system is effective at flagging risky borrowers.**

### 8. Geographic Trends

* States with **highest loan applications** also receive the **most funding**.
* **California, New York, Texas, Florida** are top funded states.

### 9. Loan Demand Over Time

* **Applications, amount received, and amount funded** all nearly **doubled by year-end** compared to the start.
* Indicates strong growth in lending demand and disbursement, supporting profitability.

### 10. Debt-to-Income (DTI)

* Most borrowers approved had **DTI < 30%**, aligning with industry practice of avoiding high-risk (>35%) DTI borrowers.

---

## 📌 Business Value of Insights

* **Risk Management:** Grading system and DTI thresholds align well with default outcomes.
* **Growth Opportunities:** Untapped loan purposes (education, medical, home improvement) and renter/mortgage-holder segments present expansion opportunities.
* **Profitability:** Rising loan demand and disbursement indicate a strong lending portfolio.
* **Portfolio Monitoring:** High-risk segments (Grades F & G) should be monitored closely or priced with higher interest/premium.

---

## 🚀 Next Steps

* Deeper **cohort analysis** (default rates by issue month).
* **Segmentation analysis** (e.g., grade × purpose) to pinpoint risky combinations.
* Create a **Power BI dashboard** with KPIs, filters (grade, state, purpose), and trend charts.

---

## 📂 Repository Structure

* `financial_loan.xlsx` → Raw dataset
* `Financial_Loans.ipynb` → EDA notebook
* `README.md` → Project overview & insights

---

## ⭐ Final Note

This project demonstrates **end-to-end EDA, data cleaning, and business insights**. It bridges technical analysis with real-world lending decisions, making it a strong portfolio project for an **entry-level Data Analyst role**.
