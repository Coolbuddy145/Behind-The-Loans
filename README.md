# 📊 Financial Loan EDA & Insights
db
## 🔎 Project Overview

This project explores a financial loans dataset to understand borrower behavior, lending patterns, and risk factors. The focus is on exploratory data analysis (EDA) — cleaning the data, analyzing it across different dimensions, and extracting insights that are meaningful for business decisions.

The analysis addresses key questions:

* What are the main purposes for which people take loans?

* How do employment length, home ownership, or DTI affect lending?

* Do loan grades reflect risk, and how do they relate to defaults and interest rates?

* Which states and borrower profiles dominate loan demand?

* How has loan demand and disbursement trended over time?

---

## ⚙️ Data Preparation

* Dropped `emp_title`, `id`, `member_id`, `total_acc` (low value).
* Converted `term` from object to integer.
* Kept outliers as they reflect real-world cases (e.g., high income, large loans).

---

## 📈 Key Insights

* **Loan Purpose:** Most loans for **debt consolidation & credit card repayment**; medical, education, and housing loans underrepresented. → Opportunity for targeted products.
* **Home Ownership:** Majority are **renters/mortgage holders**; few own homes outright. → Tailor products (home renovation for renters, investment/business loans for owners).
* **Tenure:** Only **36 & 60 month loans**, with 36 months dominating. → Preference for shorter-term, lower-risk lending.
* **Experience:** Borrowers with **10+ years work experience** receive highest loan amounts, seen as lower risk.
* **Loan Amount vs Rate:** No strong correlation; smaller loans cluster around 7–15% interest.
* **Grade & Rate:** Very strong correlation (0.94). Lower grades → higher interest rates.
* **Grade & Default Risk:** Defaults increase from A→G; Grades F & G are high-risk. → Grading system effectively flags risk.
* **Geography:** California, New York, Texas, Florida lead in applications & funding.
* **Time Trends:** Loan applications, amounts received & funded nearly **doubled by year-end**, signaling growth & profitability.
* **DTI:** Bank funds loans mainly for **DTI <30%**, avoiding high-risk borrowers (>35%).

---

## 📌 Business Value

* Confirms **grading and DTI** effectively manage risk.
* Identifies **growth opportunities** in underrepresented loan purposes & renter/mortgage-holder segments.
* Highlights **profitability trend** with rising loan demand.
* Suggests tighter monitoring of **Grades F & G**.



---


