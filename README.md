# QNB Banking Analytics | Power BI Dashboard

<p align="center">
  <b>Banking Performance, Customer Intelligence, Transaction Analytics & Credit Risk Assessment</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI" />
  <img src="https://img.shields.io/badge/Power%20Query-Data%20Transformation-5B9BD5?style=for-the-badge" alt="Power Query" />
  <img src="https://img.shields.io/badge/DAX-Business%20Logic-4472C4?style=for-the-badge" alt="DAX" />
  <img src="https://img.shields.io/badge/HTML%20%26%20CSS-Custom%20Visuals-E34F26?style=for-the-badge" alt="HTML & CSS" />
</p>

---

## 📌 Executive Overview

The **QNB Banking Analytics Dashboard** is an interactive Power BI solution designed to explore retail banking performance across customers, accounts, transactions, lending, and branch operations.

The project brings multiple banking datasets into a unified analytical model, transforming raw records into decision-support insights for customer segmentation, transaction behavior, portfolio monitoring, and credit risk assessment.

> **Data note:** This is a portfolio analytics project built with a synthetic banking dataset. The results are illustrative and do not represent actual QNB financial or operational performance.

## 🎯 Business Objectives

- Monitor customer, account, transaction, and lending performance from a consolidated view.
- Understand customer value segments and identify high-value relationships.
- Analyze transaction activity across channels, transaction types, and time periods.
- Assess loan portfolio quality and identify potential credit-risk indicators.
- Compare account balances and banking activity across branches and geographic areas.

## 📊 Dashboard Experience

The report is organized around the following analytical areas:

| Area | Business Focus |
| :--- | :--- |
| **Executive Overview** | High-level banking performance and KPI monitoring |
| **Customer Intelligence & Value Segmentation** | Customer profiles, value tiers, and contribution analysis |
| **Transaction Behavior & Digital Banking** | Transaction trends, channel mix, and customer activity |
| **Lending Portfolio & Credit Risk** | Loan status, portfolio exposure, and risk indicators |
| **Branch & Geographic Performance** | Branch-level performance and geographic comparisons |

## 💡 Selected Business Insights

| Finding | Analytical Takeaway |
| :--- | :--- |
| **VIP customers represent 10% of the customer base but contribute 57.9% of transaction value.** | Customer value is concentrated in a relatively small segment, making retention and relationship management important. |
| **ATM is the leading channel by transaction count and value.** | ATM activity is a major component of observed transaction behavior. |
| **August records the highest transaction value.** | Transaction value varies over time and should be monitored for seasonal patterns. |
| **8.3% of loans are classified as defaulted.** | Loan-status monitoring is essential for understanding portfolio quality. |
| **213 loans marked Active have passed their recorded end dates.** | These records warrant review of loan-status definitions and date-based business rules. |
| **Alexandria has the highest city-level account balance.** | Geographic balance concentration can inform branch and regional performance reviews. |

*Insights above are calculated from the project's synthetic dataset and should be interpreted within that context.*

## 🖼️ Dashboard Preview

### 1. Landing Page
<p align="center">
  <img src="./Dashboard%20Previews/Landing%20Page.png" alt="QNB Banking Analytics — Landing Page" width="95%">
</p>

### 2. Executive Summary
<p align="center">
  <img src="./Dashboard%20Previews/Summary%20Page.png" alt="QNB Banking Analytics — Summary Page" width="95%">
</p>

### 3. Accounts Analysis — Page 1
<p align="center">
  <img src="./Dashboard%20Previews/1-%20Accounts%20Page.png" alt="QNB Banking Analytics — Accounts Page 1" width="95%">
</p>

### 4. Accounts Analysis — Page 2
<p align="center">
  <img src="./Dashboard%20Previews/2-%20Accounts%20Page.png" alt="QNB Banking Analytics — Accounts Page 2" width="95%">
</p>

### 5. Transaction Analysis
<p align="center">
  <img src="./Dashboard%20Previews/Transactions%20Page.png" alt="QNB Banking Analytics — Transactions Page" width="95%">
</p>

### 6. Pricing Analysis
<p align="center">
  <img src="./Dashboard%20Previews/Pricing%20Page.png" alt="QNB Banking Analytics — Pricing Page" width="95%">
</p>

### 7. Risk Analysis
<p align="center">
  <img src="./Dashboard%20Previews/Risk%20Page.png" alt="QNB Banking Analytics — Risk Page" width="95%">
</p>

### 8. Credit Score Analysis
<p align="center">
  <img src="./Dashboard%20Previews/Score%20Page.png" alt="QNB Banking Analytics — Score Page" width="95%">
</p>

### 9. Data Model
<p align="center">
  <img src="./Dashboard%20Previews/Model.png" alt="QNB Banking Analytics — Data Model" width="95%">
</p>

## 🏗️ Data Model & Dataset

The project uses a dimensional model built from customer, account, transaction, loan, and supporting lookup datasets. The repository includes the source Excel files used by the report.

### Data files

**Fact tables**
- `fact_account.xlsx`
- `fact_loan.xlsx`
- `fact_transaction.xlsx`

**Dimension and lookup tables**
- `dim_customer.xlsx`
- `dim_date.xlsx`
- `dim_branch.xlsx`
- `dim_channel.xlsx`
- `dim_account_type.xlsx`
- `dim_loan_status.xlsx`
- `dim_loan_type.xlsx`
- `dim_transaction_type.xlsx`

## 🛠️ Tools & Technologies

- **Power BI Desktop:** Interactive report development, KPI monitoring, and data storytelling.
- **DAX:** Measures, calculated metrics, and analytical business logic.
- **Power Query:** Data cleaning, transformation, and preparation.
- **HTML & CSS:** Custom visual presentation and dashboard styling.
- **Dimensional Data Modeling:** Structured banking facts and dimensions for analytical reporting.

## 📁 Repository Structure

```text
QNB-Dashboard/
├── Assets/
│   ├── QNB Logo RGB.png
│   └── QNB Logo Solid White.png
├── Dashboard Previews/
│   ├── Landing Page.png
│   ├── Summary Page.png
│   ├── 1- Accounts Page.png
│   ├── 2- Accounts Page.png
│   ├── Transactions Page.png
│   ├── Pricing Page.png
│   ├── Risk Page.png
│   ├── Score Page.png
│   └── Model.png
├── Data/
│   ├── dim_*.xlsx
│   └── fact_*.xlsx
├── QNB.pbix
├── README.md
└── LICENSE
```

## 📜 License

This project is distributed under the MIT License. See the [LICENSE](./LICENSE) file for details.
