# Loan Default Risk Analysis — BFSI Portfolio
**Tools Used:** Python (Pandas, Matplotlib) | SQL (SQLite)
**Domain:** Banking, Financial Services & Insurance (BFSI)
**Dataset:** Loan Default Dataset — Kaggle

---

## Problem Statement
In the Indian banking sector, loan defaults directly impact profitability 
and portfolio health. This project analyses 2,55,347 loan records to 
identify high-risk borrower segments, understand default drivers, and 
recommend data-driven recovery prioritisation strategies.

---

## Key Business Insights

### 1. Overall Portfolio Health
- Total Borrowers Analysed: 2,55,347
- Total Defaults: 29,653
- Overall Default Rate: 11.61%
- Average Loan Amount: ₹1,27,579
- Average Borrower Income: ₹82,499

### 2. Highest Risk Loan Purpose
- Business loans carry the highest default rate at 12.33%
- Home loans are the safest category at 10.23%
- Recommendation: Tighten credit checks for Business and Auto loan applicants

### 3. Income vs Default Risk
- Low Income borrowers (< ₹30K) default at 21.96% — nearly 2x the average
- High Income borrowers (> ₹1L) default at only 9.10%
- Recommendation: Apply stricter DTI ratio checks for low income applicants

### 4. Employment Type Risk
- Unemployed borrowers have the highest default rate at 13.55%
- Full-time employees are the safest at 9.46%
- Recommendation: Employment stability should be a primary credit filter

### 5. Education Level Impact
- High School educated borrowers default at 12.88%
- PhD holders default at only 10.59%
- Insight: Education level correlates inversely with default risk

### 6. Risk Segmentation
| Risk Segment   | Accounts | Default Rate |
|----------------|----------|--------------|
| Very High Risk | 20,265   | 19.46%       |
| High Risk      | 20,235   | 15.96%       |
| Medium Risk    | 46,703   | 11.16%       |
| Low Risk       | 1,68,144 | 10.27%       |

- Very High Risk accounts (Low Credit Score + High Interest Rate) 
  default at nearly 2x the portfolio average
- Recommendation: Flag Very High Risk accounts for early intervention 
  and priority collection follow-up

### 7. Default vs Non-Default Borrower Profile
| Metric           | Non-Defaulted | Defaulted  |
|------------------|---------------|------------|
| Average Age      | 44.4 years    | 36.6 years |
| Average Income   | ₹83,899       | ₹71,845    |
| Average Loan     | ₹1,25,354     | ₹1,44,515  |
| Avg Credit Score | 576           | 559        |
| Avg Interest Rate| 13.18%        | 15.90%     |

- Defaulters are on average 8 years younger with lower income 
  but higher loan amounts — a classic over-leveraging pattern
- Defaulters pay 2.72% higher interest rate on average

---

## Recommendations for BFSI Risk Teams
1. Flag borrowers under age 40 with income below ₹30K for enhanced due diligence
2. Apply stricter credit limits for Business and Auto loan categories
3. Use Credit Score + Interest Rate combination for real-time risk segmentation
4. Prioritise collection follow-up on Very High Risk segment (19.46% default rate)
5. Consider employment stability as a mandatory credit filter — 
   unemployed borrowers default 43% more than full-time employees

---

## Project Structure
loan-default-analysis/
│
├── loan_default_clean.csv       # Cleaned dataset
├── loan_default_analysis.ipynb  # Jupyter notebook with all code
├── loan_default_charts.png      # Python visualisations
└── README.md                    # Project documentation

---

## Tools & Skills Demonstrated
- Data Cleaning with Pandas
- SQL queries — aggregations, CASE statements, GROUP BY, window logic
- Risk segmentation using multi-condition logic
- Business insight generation from raw data
- Data visualisation with Matplotlib
