# 📊 Financial Loan EDA & Insights

## 🔎 Project Overview

This project takes a deep dive into a financial loans dataset with the goal of understanding how people borrow, how the bank lends, and what patterns reveal about risk and performance. Instead of building predictive models, the focus here is on exploratory data analysis (EDA) — carefully cleaning the data, exploring it from multiple angles, and pulling out insights that are both practical and meaningful for the business.

Through the analysis, I looked at questions such as:

What purposes do most people take loans for?

How do factors like employment length, home ownership, or DTI influence lending decisions?

Do loan grades really capture risk, and how do they tie to defaults and interest rates?

Which states or borrower profiles account for the biggest share of loans?

How is demand trending over time?

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

## 🚀 Next Steps

