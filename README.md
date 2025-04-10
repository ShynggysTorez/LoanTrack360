# LoanTrack360: Credit Risk and Repayment Behavior Analysis

![Data](https://img.shields.io/badge/data-fintech-blue) ![Python](https://img.shields.io/badge/python-3.9-green) ![Status](https://img.shields.io/badge/project-complete-brightgreen)

## 📊 Overview

LoanTrack360 is a real-world loan analytics project focused on understanding client behavior through the lens of **credit risk and repayment patterns**.

Using real loan issuance data, scheduled repayments, and actual payment transactions, we:

- Analyzed risk dynamics over time
- Identified unpaid and underperforming loans
- Compared planned vs. actual repayments
- Created behavioral segmentation
- Built a numeric **repayment scoring system**

This project was completed as part of a technical data analyst test and is structured for professional presentation (Upwork, GitHub portfolio, dashboards).

---

## 🔧 Tools Used

- **Python** (Pandas, NumPy, Seaborn, Matplotlib)
- Jupyter Notebook
- CSV datasets (`orders.csv`, `payments.csv`, `plan.csv`)

---

## 📁 Dataset Structure

| File            | Description                                                   |
|-----------------|---------------------------------------------------------------|
| `orders.csv`    | Loan metadata: issuance dates, amounts, closure status        |
| `plan.csv`      | Scheduled cumulative payments per loan                        |
| `payments.csv`  | Actual payments made with amounts and timestamps              |

---

## 📈 Key Insights

### ✅ Step 1–2: Data Import & Feature Engineering  
Parsed timestamps, calculated loan duration, and total planned/paid amounts.

### ✅ Step 3: Risk Identification  
Flagged loans with payment gaps, created new column `payment_gap`.

### ✅ Step 4: Visualized Risk Trends  
Bar and line charts show high-risk periods by month.

### ✅ Step 5: Found Loans With Zero Payment  
Loans that are open & unpaid = direct liabilities. Total risk was quantified.

### ✅ Step 6: Planned vs Actual Payments  
Histogram visualized behavioral delta in repayments (positive = overpaid, negative = risky).

### ✅ Step 7: Segmentation  
Grouped loans into:
- **Underpaid**
- **On Track**
- **Overpaid**

With barplots and numeric summary.

### ✅ Step 8: Correlation Analysis  
Heatmap to explore connections between loan size, duration, and payment behavior.

### ✅ Step 9: Repayment Score  
Numeric scoring system (0–100) to quantify repayment behavior per loan.

---

## 🧮 Sample Visuals

<img src="assets/score_distribution.png" width="700"/>
<img src="assets/segment_barplot.png" width="700"/>
<img src="assets/risk_amount_trend.png" width="700"/>

---

## 🧠 Business Value

This project simulates the logic behind:

- Credit scoring systems
- Client risk tracking dashboards
- Collections prioritization
- Payment pattern detection
- CRM segmentation

---

## 🚀 Next Steps

- Integrate data into Power BI / Streamlit dashboard
- Train ML model for score prediction
- Recommend risk-based loan pricing tiers

---

## 📎 Project Structure

```bash
loantrack360/
│
├── analysis.ipynb              # Full notebook with analysis & visuals
├── cleaned_loans.csv           # Final dataset with repayment scores
├── assets/                     # Visuals for README and reports
└── README.md                   # Project documentation
