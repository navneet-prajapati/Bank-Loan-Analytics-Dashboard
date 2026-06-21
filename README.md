# 🏦 Bank Loan Analytics Dashboard

## 📌 Project Overview

This Power BI project analyzes a bank's loan portfolio and lending operations.

The dashboard helps stakeholders monitor:

- Loan Application Trends
- Loan Repayment Performance
- Good vs Bad Loans
- Interest Rate Analysis
- Debt-to-Income (DTI) Analysis
- State-wise Lending Distribution
- Loan Purpose Analysis

The objective is to provide actionable insights for better lending decisions and risk management.

---

# 🎯 Business Problem

Banks process thousands of loan applications every year.

Without proper monitoring, it becomes difficult to:

- Track loan performance
- Identify risky borrowers
- Analyze repayment behavior
- Monitor portfolio health
- Understand lending trends

This dashboard provides a centralized reporting solution to support data-driven lending decisions.

---

# 📂 Dataset Information

The dataset contains loan-related information including:

| Column | Description |
|----------|------------|
| ID | Unique Loan ID |
| Loan Amount | Total Loan Amount |
| Total Payment | Amount Repaid |
| Interest Rate | Interest Charged |
| DTI | Debt-To-Income Ratio |
| Loan Status | Current, Fully Paid, Charged Off |
| Purpose | Loan Purpose |
| Grade | Loan Risk Grade |
| Home Ownership | Rent, Own, Mortgage |
| State | Borrower Location |

---

# 🛠 Tools & Technologies Used

- Power BI Desktop
- Power Query
- DAX
- Excel
- Data Modeling

---

# 🧹 Data Cleaning & Preparation

### Step 1: Data Import

Imported raw loan dataset from Excel.

### Step 2: Data Validation

- Checked data types
- Verified missing values
- Removed inconsistencies

### Step 3: Date Formatting

Created:

- Month
- Quarter
- Year

Columns from Issue Date.

### Step 4: Loan Classification

Created:

#### Good Loans

- Fully Paid
- Current

#### Bad Loans

- Charged Off

---

# 📊 KPI Measures

### Total Loan Applications

```DAX
Total Loan Applications =
COUNT(Loan_Data[ID])
```

### Total Funded Amount

```DAX
Total Funded Amount =
SUM(Loan_Data[Loan Amount])
```

### Total Amount Received

```DAX
Total Amount Received =
SUM(Loan_Data[Total Payment])
```

### Average Interest Rate

```DAX
Average Interest Rate =
AVERAGE(Loan_Data[Int Rate])
```

### Average DTI

```DAX
Average DTI =
AVERAGE(Loan_Data[DTI])
```

---

# 📈 Dashboard 1 : Summary Analysis

## Dashboard Preview

![Summary Dashboard](Screenshots/Summary.png)

### Key Metrics

- Total Loan Applications
- Total Funded Amount
- Total Amount Received
- Average Interest Rate
- Average DTI Ratio

### Visuals

#### Good Loan Analysis

- Good Loan %
- Funded Amount
- Amount Received

#### Bad Loan Analysis

- Bad Loan %
- Funded Amount
- Amount Received

#### Funded Amount vs Repayment

Comparison of:

- Fully Paid
- Charged Off
- Current

#### Loan Status Analysis

Applications by Loan Status.

#### Interest Rate Analysis

Average Interest Rate by Loan Status.

#### DTI Analysis

Average DTI by Loan Status.

---

# 📈 Dashboard 2 : Overview Analysis

## Dashboard Preview

![Overview Dashboard](Screenshots/Overview.png)

### Visuals

#### Monthly Loan Applications

Monthly trend analysis.

#### State-wise Loan Analysis

Regional loan distribution using map visualization.

#### Loan Term Analysis

- 36 Months
- 60 Months

#### Home Ownership Analysis

- Rent
- Mortgage
- Own
- Other

#### Loan Purpose Analysis

- Debt Consolidation
- Credit Card
- Home Improvement
- Medical
- Educational
- Small Business
- Vacation

---

# 💡 Key Insights

### Portfolio Performance

- Total Loan Applications: 38,576
- Total Funded Amount: $435.8M
- Total Amount Received: $473.1M

### Loan Quality

- Good Loans: 86.18%
- Bad Loans: 13.82%

### Borrower Behavior

- Most borrowers belong to Mortgage and Rent categories.
- Debt Consolidation is the most common loan purpose.
- Loan applications steadily increase throughout the year.

---

# 📁 Project Structure

```text
Bank-Loan-Analytics-Dashboard
│
├── Dataset
│   └── Financial_loan_data.xlsx
│
├── Screenshots
│   ├── Summary.png
│   └── Overview.png
│
├── Bank_Loan_Analytics.pbix
│
├── Problem Statement.pdf
│
└── README.md
```

---

# 🚀 How To Use

### Step 1

Download or Clone the Repository

```bash
git clone https://github.com/yourusername/Bank-Loan-Analytics-Dashboard.git
```

### Step 2

Open Power BI Desktop

### Step 3

Open:

```text
Bank_Loan_Analytics.pbix
```

### Step 4

Refresh Data

### Step 5

Explore Dashboard Interactively

---

# 🎓 Skills Demonstrated

- Data Cleaning
- Power Query
- DAX
- Data Modeling
- KPI Development
- Banking Analytics
- Dashboard Design
- Business Intelligence
- Data Visualization
- Storytelling with Data

---

# 👨‍💻 Author

### Navneet Prajapati

Data Analyst | Power BI Developer

LinkedIn:
(Add Your LinkedIn Profile)

GitHub:
(Add Your GitHub Profile)