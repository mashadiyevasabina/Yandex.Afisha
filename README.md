# 📊 Yandex.Afisha: Marketing Cost Optimization & Data Analytics
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/İSTİFADƏÇİ_ADI/REPO_ADI/blob/main/FAYL_ADI.ipynb)

## 📌 Project Overview
This project focuses on analyzing user behavior and evaluating marketing efficiency for **Yandex.Afisha**. By examining platform visits, order histories, and marketing expenses, the goal is to optimize marketing budget allocation, improve customer retention, and maximize Return on Marketing Investment (ROMI).

---

## 🔍 Key Questions & Analytical Objectives
* **Product Performance:** How many people use the product daily, weekly, and monthly (DAU, WAU, MAU)? How long does an average session last (ASL)? What is the user retention rate over time?
* **Sales Dynamics:** When do users start buying after their first visit? How many orders do customers make, and what is the Average Order Value (AOV)? How does customer lifetime value (LTV) evolve?
* **Marketing Efficiency:** How much money was spent on marketing overall and per channel? What is the Customer Acquisition Cost (CAC) for each source? How profitable are the acquisition channels (ROMI)?

---

## 🛠 Tech Stack & Tools
* **Language:** Python 3.x
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Environment:** Jupyter Notebook / Google Colab
* **Methodologies:** Cohort Analysis, Unit Economics, Data Visualization

---

## 📁 Datasets Description

The analysis is based on three primary datasets covering the period from **June 2017 to May 2018**:

1. **`visits` (User Sessions)**
   * `User Id` — Unique user identifier
   * `Device` — User's device type (`desktop` / `touch`)
   * `Start Ts` — Session start timestamp
   * `End Ts` — Session end timestamp
   * `Source Id` — Marketing acquisition channel ID

2. **`orders` (Sales Transactions)**
   * `User Id` — Unique user identifier
   * `Buy Ts` — Transaction date and time
   * `Revenue` — Order amount in USD ($)

3. **`costs` (Marketing Expenses)**
   * `Source Id` — Marketing acquisition channel ID
   * `Dt` — Date of marketing expenditure
   * `Costs` — Amount spent on advertising in USD ($)

---

## 📈 Key Findings & Insights

### 1. Product & User Behavior
* **Session Length:** The distribution of session duration is heavily right-skewed. The **median session duration is 1–2 minutes**, indicating that users make quick decisions when searching for events or purchasing tickets.
* **Conversion Time:** **72.2% of buyers make their purchase on the very first day** of visiting the platform. Ticket purchasing is largely impulsive or goal-driven.
* **Retention:** User Retention Rate is relatively low, dropping to **4%–8% in Month 1** across most cohorts and gradually declining thereafter.

### 2. Sales & LTV
* **Order Frequency:** Repeat purchases are low, with buyers making an average of **1.16 to 1.27 orders per month**.
* **Average Order Value (AOV):** AOV remains stable throughout the customer journey, ranging between **$4.00 and $5.80**.
* **Lifetime Value (LTV):** The **June 2017 cohort** was the most valuable, reaching a cumulative LTV of **$3.02** by Month 11. However, newer cohorts (early 2018) demonstrate lower initial LTV ($0.47–$0.52 in Month 0).

### 3. Marketing Performance & ROMI
* **Ad Spend:** The largest portion of the marketing budget was spent on **Source 3** (peaking near $17,500/month in November).
* **Customer Acquisition Cost (CAC):** The most expensive channels to acquire users were **Source 3** (~$13.50) and **Source 2** (~$12.20). The cheapest channels were **Source 10** (~$4.30) and **Source 9**.
* **Return on Investment (ROMI):**
  * **Top Performers:** **Source 1** generated an exceptional ROMI (**>6000%**), followed by **Source 5** (~3500%) and **Source 2** (~2100%).
  * **Underperformers:** **Source 3** and **Source 10** failed to cross the 100% breakeven threshold, operating at a net loss.

---

<img width="1536" height="1024" alt="ChatGPT Image 1 Eyl 2026 11_37_05" src="https://github.com/user-attachments/assets/1047e90f-5342-4ad0-9276-f4f1e4ffcacb" />


## 💡 Business Recommendations

1. **Reallocate Marketing Budget:** Immediately cut or drastically scale down ad spend on **Source 3** and **Source 10**, as they fail to recover acquisition costs. Shift these funds toward high-margin channels like **Source 1** and **Source 5**.
2. **Improve Customer Retention:** Introduce loyalty programs, personalized post-purchase recommendations, and retargeting campaigns to boost repeat order frequency and user retention beyond Month 1.
3. **Optimize Conversion Funnel:** Since over 70% of purchases happen on Day 0, streamline the checkout flow (e.g., 1-click payment) and highlight trending events right on the landing page to maximize immediate conversions.
