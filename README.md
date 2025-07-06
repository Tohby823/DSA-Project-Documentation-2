# DSA-Project-Documentation-Power BI

Power BI analysis of HR data from Palmora Group, uncovering gender distribution, salary gaps, performance trends, and bonus allocations to support data-driven decision-making.

#  Power BI Project Documentation

This project is part of a capstone case study in the **Power BI Data Analysis Program**, aimed at uncovering gender-related HR issues within a Nigerian manufacturing company (**Palmora Group**) through strategic HR data visualization and insight generation.

## Project Topic: Gender Equality in the Workplace | Strategic HR Analysis at Palmora Group

### Project Overview

Palmora Group, a regional manufacturing firm based in Nigeria, was recently criticized in the media for potential gender bias in its employment practices. As an HR Data Analyst, I was tasked with investigating the organization's gender landscape using Power BI.

This analysis focuses on:
- Gender representation across departments and regions
- Gender pay gap analysis
- Salary structure compliance with a national $90,000 minimum wage regulation
- Performance rating trends by gender
- Performance-based bonus allocation and payouts

The final outcome includes a comprehensive dashboard visualizing trends, highlighting inequalities, and supporting management’s decisions with clear, actionable insights.

###  Data Sources

The primary datasets used for this analysis are:

- `Palmora Group emp-data.csv`: Contains employee information including gender, department, region, salary, and performance rating.
- `Palmora Group Bonus Rules.xlsx`: Contains business logic for assigning bonus payments based on employee performance.

These were provided as part of the HR Analytics case files.

###  Tools Used

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

###  Data Cleaning & Preparation

Key steps taken to prepare the dataset include:

- Replacing missing gender values with `"Undisclosed"`
- Removing employees with missing salaries (ex-employees)
- Dropping records with `"NULL"` departments
- Merging bonus rule data with employee dataset via performance rating
- Creating salary band groupings in increments of $10,000

---

### Exploratory HR Analysis

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

6. **Bonus and Total Pay Analysis**
   - How much bonus should each employee receive based on performance?
   - What is the total payout per region and across the company?

---

###  Visualizations & Dashboard Highlights

The Power BI dashboard includes the following visuals:

- **Donut chart**: Gender distribution by salary, count of salary by compliance status and department.
- **Pie chart**: Count of salary by compliance status and location.
- **Clustered column chart**: Salary band distribution ($10k intervals), count of gender by location, department and rating.
- **Stacked column chart**: Sum of bonus by location, sum of total pay by location.
- **Matrix**: Count of gender bt location, count of gender by department.
- **Cards**: Sum of Bonus pay and total pay by the company

---

###  Key Insights

1. Gender Distribution
 - Male-dominated in several departments and regions such as Accounting, Legal and Product Management in Abuja, Sales and Training in Kaduna and Training in Lagos.
 - Disparities most visible in the Legal, Support and Accounting departments
 - There was a significant female domination in the Research and Development department in Lagos.
2. Performance Ratings by Gender
 - "Very Good" and "Good" ratings are skewed toward females in most regions.
3. Salary Structure and Gender Pay Gap
 - Significant average salary differences observed in Legal, Business Development, Accounting and Support departments with the males receiving the average higher pay.
 - Significant average salary differences observed in Marketing and Engineering departments with the females receiving the average higher pay.
4. Salary Distribution and Minimum Wage Compliance
 - Many employees fall below the regulatory $90,000 salary threshold with a percentage of 30.97% giving the number of 292 employees.
 - Lagos region had the least compliant salaries (8.91%), next was Abuja (10.29%) then Kaduna (11.77%) with the most compliant.
5. Salary Band Distribution
   
  |Salary Range|Number of Employees|
  | ----------- | ------------------ |
  |$20000-$30000|26|
   |$30000-$40000|103|
  |$40000-$50000|105|
   |$50000-$60000|94|
   |$60000-$70000|98|
   |$70000-$80000|117|
   |$80000-$90000|108|
   |$90000-$100000|90|
   |$100000-$110000|105|
   |$110000-$120000|97|
   
6. Bonus and Total Pay Analysis
 - Bonuses are performance-linked and differ per department.
 - Top earners cluster around Business Development, Training and Marketing roles.
 - Bonus payouts highest in the Kaduna region and lowest in the Lagos region.

---

###  Bonus Salary Fomula

- `Bonus = Salary × Bonus%`
- `Total Pay = Salary + Bonus`

---

### Tools Used
- Power BI
- Microsoft Excel
- GitHub

###  Recommendations
- Improve gender balance in key departments.
- Audit and rectify gender pay gaps.
- Ensure full compliance with regulatory salary thresholds.
- Standardize performance ratings to reduce bias.

 ### Limitations
 -_ Data Duplication_: Some employees have multiple entries in the dataset, often with differing performance ratings or location assignments. This duplication could lead to inaccurate analysis of headcount, performance distribution, regional staffing, or bonus calculations, as the same individual may be counted more than once or assigned conflicting attributes.
