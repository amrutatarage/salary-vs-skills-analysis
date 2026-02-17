# Salary vs Skills Analysis (Excel Data Project)

## Project Overview
This project analyzes the relationship between technical skills, job roles, and salary trends in the 2023 data job market using advanced Excel analytics.

Objective: Transform raw job posting data into actionable insights to answer:
Which skills and roles are associated with higher compensation in data careers?

The analysis leverages Excel’s Data Model, Power Query, DAX, and PivotTables.

## Business Questions
1. Does acquiring more technical skills correlate with higher salary?
2. How does salary vary across job roles and regions?
3. What are the most in-demand skills in data-related jobs?
4. What is the salary distribution of the top 10 technical skills?

## Tools & Technologies Used
- Power Query (ETL & Data Cleaning)
- Power Pivot (Data Modeling)
- DAX (Data Analysis Expressions)
- PivotTables
- PivotCharts
- Excel Data Model

## Dataset Overview
Dataset: Real-world job postings from 2023
Includes: Job Titles, Salary Information, Job Locations, Required Skills, Employment Type

Two structured tables:
- data_jobs_all
- data_job_skills

Connected via relational model using job_id.

## Data Preparation (ETL Process)
Extract: Imported raw dataset into Power Query  
Transform: Standardized data types, cleaned text fields, removed irrelevant columns, trimmed whitespace  
Load: Loaded cleaned datasets into Excel Data Model for relational analysis  

## Data Modeling & DAX Measures
Relationship created between job postings and job skills using job_id.

Key DAX Measures:
Median Salary = MEDIAN(data_jobs_all[salary_year_avg])  
US Median Salary = CALCULATE(MEDIAN(data_jobs_all[salary_year_avg]), data_jobs_all[job_country] = "United States")

## Key Insights
1. Skills vs Salary  
   - Roles requiring broader technical stacks (Data Scientist, Senior Data Engineer) show higher median salaries.  
   - Fewer specialized skills = lower compensation.  
   - Positive relationship between number of skills and median pay.  
   Insight: Skill depth and breadth influence earning potential.  

2. Salary by Region  
   - US-based roles command higher median salaries.  
   - Differences most pronounced in senior positions.  
   - Location strongly impacts compensation.  
   Insight: Regional market maturity affects pay scales.  

3. Most In-Demand Skills  
   - Python, SQL, Tableau, Power BI, Cloud (AWS/Azure)  
   Insight: Programming and database skills remain foundational.  

4. Pay of Top 10 Skills  
   - Python and SQL = high demand + strong salary impact.  
   - Specialized database tools = high pay but lower frequency.  
   - General office tools = minimal salary influence.  
   Strategic Insight: Focus on skills at the intersection of demand and compensation.  

## What This Project Demonstrates
- End-to-end data preparation using Power Query  
- Relational data modeling in Excel  
- Writing DAX measures for business metrics  
- Building dynamic dashboards  
- Extracting career-relevant insights  
- Presenting findings through executive-style visualizations  

## Potential Extensions
- Time-based salary trend analysis  
- Skill clustering analysis  
- Country-level benchmarking dashboard  
- Power BI implementation for scalability  

## Conclusion
Excel can be used beyond spreadsheets — as a powerful analytical tool for relational models and actionable insights.  
Findings highlight the importance of technical skill development for maximizing salary potential in data careers.  
