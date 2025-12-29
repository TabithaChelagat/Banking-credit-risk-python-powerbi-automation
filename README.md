# 🏦 Banking Portfolio Risk & Asset Monitoring Dashboard

## 📌 Project Overview
This project establishes a real-time operational monitoring framework for a retail bank managing **1,000 customers**. It focuses on institutional liquidity and credit health by tracking Assets Under Management (AUM) and loan performance against strict regulatory floors. The solution leverages the **Power BI Service** to automate the reporting lifecycle and trigger proactive risk alerting via Microsoft Teams.

---

## 📊 Live Interactive Dashboard
Experience the live monitoring suite with full interactivity:
**[👉 View Live Banking Risk Dashboard](https://app.powerbi.com/view?r=eyJrIjoiMTkwNDY3NzYtMmNhZC00OThkLWFiMDktYjE1ZTAyZGYzMjRmIiwidCI6IjE0MDc0NzdmLTI1YTQtNDkzMi1hMDY4LTBlMzk0OGFjYTJiOCJ9)**

---

## 📷 Dashboard Preview
![Banking Risk Dashboard Screenshot](Dashboard)

---

## 🧠 Business Questions Answered
1.  **Capital Floor Monitoring**: Are we maintaining our required **$75M AUM floor** necessary for institutional stability?
2.  **Risk Exposure Tracking**: Is the current **Default Rate** exceeding our **7% maximum ceiling**, and what is the resulting dollar value of capital at risk?
3.  **Liquidity Balance**: Does our total loan volume of **$30.33M** provide sufficient revenue to offset the current asset shortfall?
4.  **Geographic & Segment Performance**: Which cities and risk tiers are the primary drivers of the current 13% default rate?

---

## 💡 Key Insights (Actuals vs. Targets)

| Metric | Current Actual | Target/Threshold | Status |
| :--- | :--- | :--- | :--- |
| **Default Rate** | **13%** | **7.0% (Ceiling)** | 🔴 **Critical Breach** |
| **AUM** | **$61.28M** | **$75.0M (Floor)** | 🟠 **Below Target** |
| **Total Loans** | **$30.33M** | **$15.0M (Floor)** | 🟢 **Healthy Buffer** |

* **Default Crisis**: The portfolio is currently in a high-risk state with a **13% default rate**, nearly double the established safety ceiling of 7%.
* **Capital Gap**: There is a **$13.72M shortfall** in Assets Under Management. Falling below the $75M floor limits the bank's ability to absorb further credit losses.
* **Loan Book Surplus**: Total loans of **$30.33M** show strong market activity, but the high default rate suggests that volume has been prioritized over borrower quality.

---

## 🎯 Strategic Recommendations
1.  **Immediate Credit Tightening**: Halt new originations for high-risk segments until the **Default Rate** trends back toward the 7% goal.
2.  **Incentivized Deposit Growth**: Launch high-yield asset acquisition campaigns to bridge the **$13.72M AUM gap** and restore capital stability.
3.  **Regional Risk Audit**: Use the **City Performance** visuals to identify and cap lending in regional "hotspots" contributing to the 13% default rate.

---

## 🔄 BI Automation & Proactive Alerting
To eliminate manual monitoring and ensure 24/7 oversight, the following automation has been deployed:
* **Scheduled Refresh**: Dataset is connected to **Google Drive** via the **Web Connector**, with an automated refresh daily at **6:00 PM**.
* **Stakeholder Subscriptions**: Risk Committee receives an automated executive PDF every **Monday at 9:00 PM**.
* **Real-Time Microsoft Teams Alerts**: Triggered immediately when critical thresholds are reached:
    * **Alert**: Default Rate drops to **7%** (Achievement Notification).
    * **Alert**: Active Loans drop to **$15M** (Critical Liquidity Floor).
    * **Alert**: AUM reaches **$75M** (Capital Floor Achievement).

---

## 🛠️ Technical Stack
* **Data Sourcing**: **Google Drive** integrated via **Web Connector** for seamless cloud-to-cloud data transfer.
* **ETL & Cleaning**: Utilized **Power Query** to perform advanced data transformation, handling null values and normalizing credit tiers.
* **Power BI**: Star Schema data modeling and advanced **DAX** for portfolio KPIs.
* **Power Automate**: Integration for automated stakeholder alerting.

---
*Project Completed by Tabitha Chelagat as part of a Data Analytics Portfolio.*
