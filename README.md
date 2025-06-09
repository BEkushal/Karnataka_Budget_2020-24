# 📊 Karnataka State Budget (2020–2024) – Public Account Analysis

## 🧾 Project Overview

This project is a comprehensive analysis of Karnataka's state budget data spanning from financial years **2020–21 to 2023–24**, based on data extracted from the publicly available **Annual Financial Statements (AFS)** documents to derive insights about the state's financial priorities, execution trends, and fiscal performance across Revenue, Capital, and Public Accounts. The final product is structured to support data-driven storytelling suitable for policymakers, analysts, and the general public.

Unlike Revenue and Capital accounts, **Public Account transactions are not government income or expenditure per se**, but **liabilities and recoveries held temporarily in trust**—requiring careful consideration while analyzing.

---

## 🔍 Objectives

- Analyze the trends and patterns across **Revenue**, **Capital**, and **Public Accounts**.
- Identify **estimation gaps** between BE(Budget Estimates), RE(Revised Estimates), and Actuals.
- Highlight **overperforming and underperforming** sectors/sub-categories.
- Detect and document **outliers** and anomalies.
- Assess the government's financial priorities over time
- Provide **actionable insights** in a professional, readable, and accessible format.

---

## 📂 Folder Structure & Sheet Organization

- **Receipts** – Raw data from the AFS receipts table.
- **Expenditure** – Raw data from the AFS disbursement table.
- **Deficit_Surplus** – Year-wise surplus/deficit status for Revenue, Capital, and Public accounts.
- **BE_Priorities** – Holds the Budget Estimates (BE) of different account heads and their sub-categories belonging Revenue, Capital, and Public Accountsto under **Disbursements**.
- **RE_Analysis** – Same structure as BE_Priorities, but for Revised Estimates (RE) under **Disbursements**.
- **BE_vs_RE_Corrections** – Differences between BE and RE across years and Accounts under **Disbursements**.
- **Execution_Vs_BE** – Analysis of actuals vs BE under **Disbursements**.
- **Execution_Vs_RE** – Analysis of actuals vs RE under **Disbursements**.
- **BE_Receipts_Priorities** – Holds the Budget Estimates (BE) of different account heads and their sub-categories belonging Revenue, Capital, and Public Accountsto under **Receipts**.
- **RE_Receipts_Analysis** - Same structure as BE_Receipts_Analysis, but for Revised Estimates (RE) under **Receipts**.
- **Receipts_BE_Vs_RE_Corrections** - Differences between BE and RE across years and Accounts under **Receipts**.
- **Receipts_Execution_Vs_BE** - Analysis of actuals vs BE under **Receipts**.
- **Receipts_Execution_Vs_RE** - Analysis of actuals vs RE under **Receipts**.
- **Public_BE_Priorities** – Holds BE of different account heads and their sub-categories for **Receipts** under the Public Account.
- **Public_RE_Analysis** – Same structure as BE_Priorities, but for Revised Estimates (RE).
- **Public_BE_vs_RE_Corrections** – Differences between BE and RE across years for **Receipts** under the Public Account.
- **Public_Execution_vs_BE (Receipts)** – Analysis of actuals vs BE for **Receipts** under the Public Account.
- **Public_Execution_vs_RE (Receipts)** – Actuals vs RE for **Receipts** under the Public Account.
- **Public_BE_Disb_Priorities** – Holds BE of different account heads and their sub-categories for  **Disbursements** under the Public Account.
- **Public_RE_Disb_Analysis** – Holds RE of different account heads and their sub-categories for  **Disbursements** under the Public Account.
- **Public_BE_RE_Disb_Corrections** - Differences between BE and RE across years for **Disbursements** under the Public Account.
- **Public_Disb_Execution_vs_BE** - Analysis of actuals vs BE for **Disbursements** under the Public Account.
- **Public_Disb_Execution_vs_RE** - Analysis of actuals vs RE for **Disbursements** under the Public Account.
- **Insights_Summary** – Consolidated insights across all sheets.

---

## 🧠 Methodology & Key Considerations

### 🔹 Data Sources
- for **FY 2020-21**: https://finance.karnataka.gov.in/storage/pdf-files/03-AnnualFinStatement-2021-22.pdf
- for **FY 2021-22**: https://finance.karnataka.gov.in/storage/pdf-files/AFS%202022-23.pdf
- for **FY 2022-23**: https://finance.karnataka.gov.in/storage/pdf-files/3_AFSJULY2023-24.pdf
- for **FY 2023-24**: https://finance.karnataka.gov.in/storage/pdf-files/3_AFS2024-25.pdf

### 🔹 Data Handling
- Data was manually extracted from AFS PDFs for the years 2020–2024.
- The data for current FY is sourced from the AFS of the subsequent year, eg:- for FY 2022-23 data is extracted from AFS 2023-24
- Only columns **Heads of Account**, **BE of cuurent FY** and **RE of current FY** are extracted from the relavant AFS.
- All monetary values were standardized in **Indian Number System** and converted with an understanding that AFS values are recorded in **lakhs**.
- Although **Contingency Fund** is a different account head altogether but, it's considered under Revenue Account in the Analysis.
- Not all Sub-categories or Sub-account heads of the main account heads like **Social Services**,**Economic Services** etc are extracted from the AFS due to inconsistent availabilty across years.
- Due to missing account heads & their sub-categories across years, aggregated figures are extracted maintaining data consistency.

### 🔹 Structuring for Analysis
- All analysis sheets followed a **structured pivot table format** for consistency.
- Separate analyses were maintained for **Receipts vs Expenditures** due to their differing interpretations across all the 3 Accounts (Revenue, Capital & Public).
- Year-wise, Sector-wise, and Sub-category-level granularity was ensured.

### 🔹 Currency Formatting
- Values were cross-verified for correctness in crore/lakh/rupee conversions.
- Anomalies in earlier formats were rectified before deriving insights.

---

## 💡 Notable Insights

### 📌 From `Deficit_Surplus`
- **Revenue & Capital Accounts** displayed consistent deficits.
- Both Accounts witness a sharp spike in deficits in FY 2023-24.
- **Fiscal deficit** showed a sharp increase in FY 2022-23 and dropped down by 17.1% marking a considerable imporvement.

### 📌 From `BE_Priorities` and `RE_Analysis`
- **Social Services** (Revenue Account) and **Capital Expenditure** (Capital Account) are consistently prioritised, showing significant growth over the years.
- **Grants in aid and contributions** (Revenue Account) and **Capital disbursement outside revenue account** (Capital Account) are less prioritised.

### 📌 From `Execution_Vs_BE` and `Execution_Vs_RE`
- **Capital Account of General Economic Services** account head under **Capital Expenditure** belonging to **Capital Account** showed a massive overspending of 634.04% in FY 2022-23.
- In FY 2021-22 an anamolousobservation was spotted by **Capital Account of General Economic Services** (sub-category of Capital Expenditure) having BE as ₹-52.34 crores leading to -1663.99% utilization.
- **Capital Account of General Economic Services** (sub-category of Capital Expenditure) hit -2172.99% of RE, signaling massive overspending in 2021-22.


### 📌 From `BE_Receipts_Priorities` and `RE_Receipts_Analysis`
- **Tax Revenue** (Revenue Account) and **Capital Receipts** (Capital Account) remained top sources of revenue across all years.
- **Non Tax Revenue** (Revenue Account) and **Miscellaneous Capital Receipts** (Capital Account) within Capital receipts remained the bottom sources of revenue to the government across all the years.

### 📌 From `Public_Execution_Vs_BE` and `Public_Disb_Execution_Vs_BE`
- **Deposits Bearing Interest** within **Deposit & Advance** showed a massive execution of 27495.35% of BE for **Receipts** and 37766.38% of BE for **Disbursements** in FY 2022-23.

---

## 🚀 Final Thoughts
- This project is designed not just as a static report but as a portfolio-grade demonstration of analytical rigor, fiscal understanding, and storytelling. While Public Account was treated as supporting data, the heart of the analysis lies in how Revenue and Capital were planned, modified, and executed. Outliers like the Contingency Fund deviation and extremely high execution percentages in Suspense accounts have been highlighted.
- The analysis aims to spark deeper interest in fiscal transparency and to support citizens and analysts in making sense of complex government budgeting with clarity and confidence.

---

## 📎 Acknowledgements

- Data Source: **Annual Financial Statements** of Karnataka State Government (2020–2024) mentioned above under **Methodology & Key Considerations**.
- Analysis conducted using **Microsoft Excel** with Pivot Tables, Conditional Formatting, Functions, Calculated Fields and Manual Insights.
