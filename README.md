# 📊 HR Analytics: Employee Attrition & Retention Intelligence

## 📌 Project Overview
Employee turnover is one of the most critical challenges facing modern enterprises, impacting team continuity, organizational productivity, and operating margins. 

This project provides an end-to-end commercial **HR Analytics & Employee Attrition Intelligence System** analyzing enterprise workforce patterns across **1,470 employee records** and **35 attributes**. Built using **Advanced Microsoft Excel**, **Interactive Python EDA**, and **Executive Dashboarding**, the project uncovers root causes of resignation, quantifies risk multipliers, and delivers actionable corporate retention recommendations.

---

## 🛠️ Tools & Technologies Used
- **Microsoft Excel (Advanced)**: Multi-tab commercial financial & HR modeling, automated Pivot Tables, dynamic formulas (`SUM`, `AVERAGE`, `COUNTIFS`, nested ratios), custom number formatting (`$#,##0`, `0.0%`), frozen audit panes, and embedded executive openpyxl charts.
- **Python (Pandas, NumPy, Matplotlib, Seaborn)**: Rigorous exploratory data analysis (EDA), data hygiene pipelines, feature engineering, and statistical distribution plotting.
- **Jupyter Notebook**: Fully documented interactive analysis walkthrough with code, plots, and executive takeaways.

---

## 📂 Repository Structure & Files
| File Name | Format | Description |
| :--- | :--- | :--- |
| `HR_Analytics_Attrition_Master_Analysis.xlsx` | `.xlsx` | Enterprise-grade 5-tab Excel workbook with Executive Dashboard, Pivot Summaries, Comparative Matrices, and Cleaned Data. |
| `HR_Analytics_Attrition_Analysis.ipynb` | `.ipynb` | Comprehensive Python Jupyter Notebook with end-to-end statistical EDA and visualizations. |
| `HR-Employee-Attrition.csv` | `.csv` | Original enterprise source dataset (1,470 employee records, 35 columns). |
| `README.md` | `.md` | Full repository documentation, analytical methodology, findings, and strategic retention framework. |

---

## 📑 Excel Architecture (`HR_Analytics_Attrition_Master_Analysis.xlsx`)
The master Excel workbook is structured into five logically separated worksheets:

### 1. `Executive_Dashboard`
- **Executive KPI Cards**:
  - **Total Headcount**: 1,470 employees
  - **Active Employees**: 1,233 (83.9%)
  - **Attrited Employees**: 237 departures
  - **Overall Attrition Rate**: **16.1%**
  - **Average Monthly Income**: **$6,503**
- **Embedded Dynamic Charts**:
  - *Department Turnover: Active vs. Attrited Headcount (Column Chart)*
  - *Attrition Rate by Job Role Ranking % (Horizontal Bar Chart)*
  - *OverTime Turnover Acceleration: Regular vs. OverTime (Clustered Column Chart)*
  - *Attrition Distribution by Marital Status (Pie Chart)*

### 2. `Pivot_Summary`
- **Table 1: Department Analysis**: Headcount, active vs. attrited employees, turnover rate, and average monthly income.
- **Table 2: Job Role Turnover & Compensation Ranking**: Ranks all 9 job roles by attrition risk and cross-references against average compensation and job satisfaction scores.
- **Table 3: Age Demographics & Experience**: Breaks down attrition by age brackets (18–25, 26–35, 36–45, 46–55, 55+), tracking average company tenure and total working experience.
- **Table 4: Work-Life Balance Rating Matrix**: Evaluates retention rates across satisfaction ratings (Level 1 Low to Level 4 Best).

### 3. `Comparative_Analysis`
- **Comparison 1: OverTime Acceleration Matrix**: Cross-tabulates departments against OverTime status, calculating the exact **Turnover Risk Multiplier**.
- **Comparison 2: Marital Status & Gender Turnover Matrix**: Evaluates attrition rates across Single, Married, and Divorced cohorts by gender.
- **Comparison 3: Monthly Income Bracket vs. Equity Retention**: Analyzes attrition rates across compensation brackets (<$3K, $3K-$6K, $6K-$10K, $10K+) and correlates with stock option levels.

### 4. `Cleaned_Data`
- Sanitized dataset with non-informative zero-variance fields removed (`EmployeeCount`, `StandardHours`, `Over18`).
- Engineered derived analytical features: `Attrition_Flag`, `Age_Group`, `Income_Bracket`, and `Total_Satisfaction_Score`.

### 5. `Master_Raw_Data`
- Complete, unaltered transactional log preserved for auditing, governance, and data lineage.

---

## 📈 Key Business Insights & Findings

### 1. OverTime is the #1 Catalyst of Resignation (3.0x Risk Multiplier)
- Employees working **OverTime experience a 30.5% attrition rate** (127 departures / 416 employees).
- In contrast, employees working **Regular Hours have a low 10.4% attrition rate** (110 departures / 1,054 employees).
- **Overtime workers represent only 28.3% of the total headcount, yet account for 53.6% of all resignations**.

### 2. Job Role Vulnerability & Compensation Disparity
- **Sales Representatives** face an alarming **39.8% attrition rate** (lowest average income: **$2,626/mo**).
- **Laboratory Technicians** experience **23.9% attrition** (average income: **$3,237/mo**).
- **Human Resources** staff experience **23.1% attrition** (average income: **$4,236/mo**).
- Senior leadership roles (**Managers at 4.9%** and **Research Directors at 2.5%**) enjoy exceptional stability, earning over $16,000/mo.

### 3. Early Career & Single Cohort Mobility
- **Age 18–25 Cohort**: Experiences the highest generational attrition at **35.8%**, reflecting early-career job switching.
- **Age 26–35 Cohort**: Forms the largest workforce volume (606 employees) and accounts for nearly half of all exits (**116 attrited, 19.1% rate**).
- **Marital Status**: **Single employees leave at 25.5%**, more than double that of married (12.5%) and divorced (10.1%) peers.

### 4. Work-Life Balance & Burnout Thresholds
- Employees who rated their Work-Life Balance as **Level 1 (Poor) suffered a 31.3% attrition rate**.
- Employees reporting higher Work-Life Balance (Levels 2–4) maintained stable attrition between 14.2% and 17.6%.

---

## 💡 Strategic Retention Action Plan for Leadership

1. **Overtime Workload Capping**:
   - Establish mandatory thresholds for overtime hours and introduce compensatory time-off (comp-time) for critical project sprints.
2. **Targeted Entry-Level Salary Restructuring**:
   - Benchmark and elevate starting compensation for Sales Representatives and Laboratory Technicians to market median ($3,800 - $4,200).
3. **Early-Tenure Retention Incentives (Ages 18–30)**:
   - Provide structured 12-to-18-month career progression roadmaps, tuition assistance, and rotational mentorship programs to stem early career exits.
4. **Equity & Stock Option Vesting**:
   - Extend Level 1 stock option grants to mid-level individual contributors, significantly dampening voluntary turnover.

---

## 🚀 How to Run the Project
1. **Excel Model**:
   - Open `HR_Analytics_Attrition_Master_Analysis.xlsx` in Microsoft Excel (2016 or newer / Office 365).
   - Explore the `Executive_Dashboard` tab for visual summaries, or inspect `Comparative_Analysis` and `Pivot_Summary` for formulas.
2. **Python Notebook**:
   - Open `HR_Analytics_Attrition_Analysis.ipynb` in Jupyter Notebook, JupyterLab, or VS Code.
   - Run all cells sequentially (`Kernel -> Restart & Run All`) to reproduce all plots and statistical tables.

---

## 👤 Author
**Sagar Kale**  
*Data Operations & MIS Specialist*
