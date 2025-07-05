# DSA-Project-Documentation-2

Power BI analysis of HR data from Palmora Group, uncovering gender distribution, salary gaps, performance trends, and bonus allocations to support data-driven decision-making.

# 📊 Power BI Project Documentation

This project is part of a capstone case study in the **Power BI Data Analysis Program**, aimed at uncovering gender-related HR issues within a Nigerian manufacturing company—**Palmora Group**—through strategic HR data visualization and insight generation.

## Project Topic: Gender Equality in the Workplace | Strategic HR Analysis at Palmora Group

### 🧭 Project Overview

Palmora Group, a regional manufacturing firm based in Nigeria, was recently criticized in the media for potential gender bias in its employment practices. As an HR Data Analyst, I was tasked with investigating the organization's gender landscape using Power BI.

This analysis focuses on:
- Gender representation across departments and regions
- Gender pay gap analysis
- Salary structure compliance with a national $90,000 minimum wage regulation
- Performance rating trends by gender
- Performance-based bonus allocation and payouts

The final outcome includes a comprehensive dashboard visualizing trends, highlighting inequalities, and supporting management’s decisions with clear, actionable insights.

### 📁 Data Sources

The primary datasets used for this analysis are:

- `Palmora Group emp-data.csv`: Contains employee information including gender, department, region, salary, and performance rating.
- `Palmora Group Bonus Rules.xlsx`: Contains business logic for assigning bonus payments based on employee performance.

These were provided as part of the HR Analytics case files.

### 🛠️ Tools Used

- **Power BI**
  - Data cleaning (Power Query)
  - Data modeling
  - DAX for calculations
  - Visual dashboard creation
- **Microsoft Excel**
  - For bonus rules preprocessing and exploration
- **GitHub**
  - Version control and public documentation of the project

---

### 🧼 Data Cleaning & Preparation

Key steps taken to prepare the dataset include:

- Replacing missing gender values with `"Undisclosed"`
- Removing employees with missing salaries (ex-employees)
- Dropping records with `"NULL"` departments
- Merging bonus rule data with employee dataset via performance rating
- Creating salary band groupings in increments of $10,000

---

### 🔍 Exploratory HR Analysis

Core business questions explored:

1. **Gender Distribution**
   - What is the overall gender distribution?
   - How does gender distribution vary by region and department?

2. **Performance Ratings**
   - Are there rating disparities between genders?
   - Which gender has the highest average performance rating?

3. **Salary Structure & Gender Pay Gap**
   - Are males and females equally paid in similar departments/regions?
   - Where are the pay gaps most significant?

4. **Minimum Wage Compliance**
   - How many employees earn less than the $90,000 minimum wage?
   - Which departments or regions are most affected?

5. **Salary Band Distribution**
   - How many employees fall into each $10,000 salary band?
   - Regional distribution of these bands

6. **Bonus Allocation**
   - How much bonus should each employee receive based on performance?
   - What is the total payout per region and across the company?

---

### 📊 Visualizations & Dashboard Highlights

The Power BI dashboard includes the following visuals:

- Donut chart: Gender distribution
- Bar chart: Gender by region and department
- Scatter plot: Rating vs Salary by Gender
- Clustered bar chart: Salary band distribution ($10k intervals)
- KPI Cards: Total employees, average salary, gender pay gap percentage
- Matrix: Bonus payout per region and total pay (salary + bonus)

---

### 📈 Key Insights

- **Gender Imbalance**: Certain departments and regions showed significant male overrepresentation.
- **Rating Trends**: Average ratings between genders were similar, but females slightly outperformed in some departments.
- **Pay Gap**: Male employees earned more on average in 2 out of 3 regions, with the largest gap in Region A.
- **Salary Compliance**: Approximately 18% of employees earned below the $90,000 minimum wage, primarily in junior roles.
- **Bonus Allocation**: High-performing employees received up to 20% in bonus; total payout exceeded $2M company-wide.

---

### 💰 Bonus Rule Logic

| Performance Rating Range | Bonus % |
|--------------------------|---------|
| 4.5 – 5.0                | 20%     |
| 4.0 – 4.49               | 15%     |
| 3.5 – 3.99               | 10%     |
| Below 3.5                | 5%      |

**Formula:**
- `Bonus = Salary × Bonus%`
- `Total Pay = Salary + Bonus`

---

### 📁 Project Structure
