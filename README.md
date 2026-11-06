# Kast: Real-Time AML & Wallet Drain Surveillance 🛡️

[![View Dashboard](https://img.shields.io/badge/View_Dashboard-Tableau_Public-blue?style=for-the-badge&logo=tableau)]([Insert your Tableau Public Link Here])

## 📌 Project Overview
This project simulates a real-time risk operations environment for a financial technology platform. Utilizing the PaySim dataset, this dashboard is designed for executive oversight and analyst triage of high-volume money laundering (AML) and wallet drain attempts.

The objective of this project was to transform raw, highly-abstracted synthetic transaction logs into an executive-ready operational dashboard that tracks total financial exposure and isolates malicious behavioral spikes from normal baseline volume.

## 📊 The Dashboard
**[🔗 Click here to interact with the live Tableau dashboard] https://public.tableau.com/app/profile/milena.obilinovic8793/viz/AML_Wallet_Drain_Surveillance/Dashboard1**

### Key Features
*   **Executive KPI Scorecard:** High-level metrics tracking **Total Financial Exposure** and **Total Actionable Alerts**, formatted for immediate leadership consumption.
*   **Risk Over Time (Fraud vs. Baseline):** A continuous time-series area chart that maps transaction volume across a calendar timeline. It utilizes categorical color-coding to instantly isolate malicious wallet-drain spikes from legitimate baseline volume.
*   **Data Translation:** Converted raw, abstracted machine-learning data (e.g., operational "Steps") into realistic business dimensions (UTC Timestamps, Billions/Millions financial formatting, and actionable Tooltips).

## 🗄️ The Data
This project utilizes **PaySim**, a synthetic dataset generated using an agent-based simulation approach to mimic normal and malicious mobile money transactions. 
*   **Volume:** +6 Million transactions.
*   **Typologies Targeted:** 
    *   *Wallet Drains / Account Takeovers:* Rapid depletion of origin balances transferred to mule destinations.
    *   *Layering:* High-velocity movement of illicit funds designed to evade standard threshold rules.
*   *Note: Due to the synthetic nature of the dataset designed for privacy compliance, geographic and identifiable metadata were intentionally omitted.*

## 🛠️ Technical Implementation
*   **Tool:** Tableau Public
*   **Data Engineering / Calculated Fields:** 
    *   Implemented `DATEADD` functions to convert abstract operational hours into standard calendar timelines.
    *   Custom dimension clustering to separate confirmed fraud flags from baseline volume.
    *   Number formatting rules to compress multi-billion dollar transaction clusters into readable executive figures.
*   **Design Philosophy:** Strict adherence to data-ink ratio best practices. Removed default gridlines, optimized visual hierarchy, and utilized fixed-pixel dashboard scaling to ensure consistent rendering across web environments.

## 💡 Use Case & Business Value
In a live FinTech environment, this dashboard architecture allows a Head of Risk to:
1.  **Monitor systemic health** by observing the ratio of legitimate volume to flagged anomalies.
2.  **Size the financial risk** of active attacks in real-time.
3.  **Allocate analyst headcount** dynamically based on volume spikes in the triage queue.

---
*Created by Milena Obilinovic — linkedin.com/in/milenaobi*
