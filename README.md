# 🏦 QNB Retail Banking Analytics | Power BI Dashboard

<p align="center">
  <b>Banking Performance, Customer Intelligence, Lending Portfolio & Credit Risk Analysis</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI" />
  <img src="https://img.shields.io/badge/Power%20Query-Data%20Transformation-5B9BD5?style=for-the-badge" alt="Power Query" />
  <img src="https://img.shields.io/badge/DAX-Business%20Logic-4472C4?style=for-the-badge" alt="DAX" />
  <img src="https://img.shields.io/badge/HTML%20%26%20CSS-Custom%20Visuals-E34F26?style=for-the-badge" alt="HTML & CSS" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="MIT License" />
</p>

---

## 📌 Executive Overview

The **QNB Retail Banking Analytics Dashboard** is an interactive Power BI portfolio project covering customers, accounts, transactions, lending, branch operations, loan pricing, and credit risk. It brings several banking datasets into one analytical model to support portfolio monitoring, customer segmentation, and operational review.

The report includes custom HTML/CSS visuals authored through DAX measures alongside native Power BI visuals. The data supplied with this project is synthetic and its results are illustrative; they do not represent actual QNB financial or operational performance.

## 🎯 Business Objectives

- Monitor customer, account, transaction, and lending performance from a consolidated view.
- Compare customer segments and their contribution to account balances and transaction activity.
- Analyze transaction volume and value across channels, transaction types, and time.
- Review loan status, risk segments, debt-to-income indicators, and pricing patterns.
- Compare account balances and branch activity across cities and account types.

## 📊 Dataset Snapshot

The workbook data contains **1,000 customers**, **1,243 accounts**, **4,000 transactions**, and **600 loans**, supported by reference tables for dates, branches, channels, and banking product classifications.

| Area | Dataset observation |
| :--- | :--- |
| **Accounts** | 299.42M total account balance across 1,243 accounts |
| **Customer segments** | 100 VIP, 300 Mass, and 600 Retail customers |
| **Lending** | 237.40M total loan amount; 50 of 600 loans are marked Defaulted (8.33%) |
| **Transactions** | 74.36M total transaction amount across 4,000 records |
| **Branches** | 20 branches and 506 employees |

*Amounts are presented in the dataset's units. The source data does not specify a currency.*

## 💡 Selected Insights

| Finding | Analytical takeaway |
| :--- | :--- |
| **VIP customers are 10% of the customer base and hold 70.25% of account balances.** | Deposit balances are concentrated in a small customer segment. |
| **High-risk loans default more often, while average rates are similar across risk buckets.** | The dataset suggests limited differentiation in observed pricing by modeled risk tier; this is descriptive, not a causal conclusion. |
| **62 loans have a DTI of at least 43%, representing 44.43% of total loan amount.** | The high-DTI subset merits closer underwriting review. |
| **ATM has the highest transaction count and transaction value among the three channels.** | Channel activity can be compared by both volume and value. |
| **November has the highest transaction value among the months in the supplied data.** | Transaction value varies over time and can be explored by the report's date analysis. |
| **Mansoura has the highest city-level account balance in the supplied data.** | Branch and city balance concentration can inform geographic performance reviews. |

*Insights are calculated from the included synthetic workbook data. Risk tiers and thresholds are fields or assumptions in the dataset and should not be interpreted as regulatory guidance.*

## 🖼️ Dashboard Preview

### 1. Landing Page
<p align="center">
  <img src="./Dashboard%20Previews/Landing%20Page.png" alt="QNB Banking Analytics — Landing Page" width="95%">
</p>

### 2. Executive Summary
<p align="center">
  <img src="./Dashboard%20Previews/Summary%20Page.png" alt="QNB Banking Analytics — Summary Page" width="95%">
</p>

### 3. Accounts Analysis — View 1
<p align="center">
  <img src="./Dashboard%20Previews/1-%20Accounts%20Page.png" alt="QNB Banking Analytics — Accounts Analysis, View 1" width="95%">
</p>

### 4. Accounts Analysis — View 2
<p align="center">
  <img src="./Dashboard%20Previews/2-%20Accounts%20Page.png" alt="QNB Banking Analytics — Accounts Analysis, View 2" width="95%">
</p>

### 5. Transactions Analysis
<p align="center">
  <img src="./Dashboard%20Previews/Transactions%20Page.png" alt="QNB Banking Analytics — Transactions Analysis" width="95%">
</p>

### 6. Portfolio Analysis
<p align="center">
  <img src="./Dashboard%20Previews/Portfolio%20Page.png" alt="QNB Banking Analytics — Portfolio Analysis" width="95%">
</p>

### 7. Risk Analysis
<p align="center">
  <img src="./Dashboard%20Previews/Risk%20Page.png" alt="QNB Banking Analytics — Risk Analysis" width="95%">
</p>

### 8. Pricing Analysis
<p align="center">
  <img src="./Dashboard%20Previews/Pricing%20Page.png" alt="QNB Banking Analytics — Pricing Analysis" width="95%">
</p>

### 9. Credit Score Analysis
<p align="center">
  <img src="./Dashboard%20Previews/Score%20Page.png" alt="QNB Banking Analytics — Credit Score Analysis" width="95%">
</p>

### 10. Data Model
<p align="center">
  <img src="./Dashboard%20Previews/Model.png" alt="QNB Banking Analytics — Data Model" width="95%">
</p>

## 🏗️ Data Model & Dataset

The model combines three transaction-level fact tables with customer, date, branch, channel, and product/status lookup tables.

**Fact tables**
- `fact_account.xlsx` — account balances, rates, opening dates, and foreign keys.
- `fact_loan.xlsx` — loan amounts, principal, dates, status/type keys, risk attributes, and DTI fields.
- `fact_transaction.xlsx` — transaction amounts, dates, account keys, channel keys, and transaction-type keys.

**Dimension and lookup tables**
- `dim_customer.xlsx` — customer attributes and segment.
- `dim_date.xlsx` — calendar attributes for time analysis.
- `dim_branch.xlsx` — branch, city, staffing, and opening-date attributes.
- `dim_channel.xlsx` — ATM, Branch, and Online channel labels.
- `dim_account_type.xlsx` — account type labels.
- `dim_loan_status.xlsx` — Active, Closed, and Defaulted status labels.
- `dim_loan_type.xlsx` — loan product labels.
- `dim_transaction_type.xlsx` — Deposit, Withdrawal, Transfer, and Payment labels.

## 🛠️ Tools & Technologies

- **Power BI Desktop:** Interactive report development and data visualization.
- **DAX:** Measures, calculated metrics, risk analysis, and business logic.
- **Power Query:** Data cleaning, transformation, and preparation.
- **HTML & CSS:** Custom visual presentation embedded in report measures.
- **Dimensional modeling:** Related fact and lookup tables for banking analysis.

## 🚀 Getting Started

1. Clone or download this repository.
2. Open `QNB.pbix` in Power BI Desktop.
3. If Power BI prompts for data sources, point the queries to the Excel workbooks in the `Data/` folder and refresh the model.
4. Use the report navigation and slicers to explore customer, account, transaction, portfolio, risk, pricing, and score analysis.

The repository includes the `.pbix` report file and source workbooks. The PBIP project archive supplied separately is not part of the current repository contents.

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
│   ├── Portfolio Page.png
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

## 📜 License & Author

- **Author:** Kerelos Nakhla ([GitHub Profile](https://github.com/Kerelos-Nakhla) • [Portfolio](https://kerelos-nakhla.github.io/Portofolio/))
- **License:** MIT License. See [LICENSE](./LICENSE) for details.
