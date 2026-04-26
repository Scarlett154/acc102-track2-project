# Data Science Job Market Analysis: Skills, Salaries, and Career Strategy

## 1. Problem & User
Data science professionals face uncertainty about which technical skills to prioritize for career advancement. This project analyzes real job market data to provide actionable insights for job seekers on skill investment strategies, while offering HR teams and educators data-driven benchmarks for salary planning and curriculum design.

## 2. Data
* **Source**: [Data Science Job Postings with Salaries (2025)](https://www.kaggle.com/datasets/elahehgolrokh/data-science-job-postings-with-salaries-2025/data) | Kaggle
* **Access Date**: 2026-04-20
* **Key Fields**:
  * `salary`: Annual salary range (in EUR, converted to midpoint for analysis)
  * `skills`: Extracted list of required technical skills
  * `seniority_level`: Experience classification (Junior/Mid/Senior/Lead)
  * `job_title`: Position title for role categorization
* **Dataset**: ~2,500 data science positions, primarily from U.S. tech markets
* **License**: CC0 Public Domain

## 3. Methods
* **Data Processing**:
  * Cleaned salary data by converting string ranges to numerical midpoints
  * Parsed and standardized comma-separated skill lists
  * Handled missing values and performed consistency checks
* **Analytical Steps**:
1. **Salary Distribution Analysis**: Statistical summary and visualization of overall salary ranges
2. **Seniority Segmentation**: Group analysis by experience level with comparative statistics
3. **Skills Frequency Analysis**: Count and rank most commonly required skills
4. **Skills Premium Calculation**: Compute average salary premium for each skill
5. **Popularity-Salary Correlation**: Scatter plot and correlation analysis
6. **Skill Count Analysis**: Relationship between number of skills and salary levels

* **Visualization**: Matplotlib/Seaborn for all six core charts with consistent styling

## 4. Key Findings
* **Seniority Drives Salary**: Senior roles command 40-60% premium over entry-level positions, with clear progression tiers
* **Skill Popularity ≠ High Pay**: Common skills (Python, SQL) are foundational but offer lower premiums, while specialized skills (MLOps, Spark) command 20-35% higher salaries
* **Optimal Skill Count**: Positions requiring 5-7 core skills show strongest salary-to-requirement ratio, with diminishing returns beyond 8+ skills
* **High-Value Specializations**: Machine Learning Engineering, Data Engineering, and cloud infrastructure skills consistently rank among highest-paying
* **Strategic Career Path**: Early-career professionals should master common skills first, then specialize in 1-2 high-premium areas for mid-career growth

## 5. How to Run
This project is designed to be highly reproducible. No local data download is required.

1. Clone or download this repository.
2. Ensure you have a Python environment installed with the following libraries: pandas, numpy, matplotlib, and seaborn.
3. Open notebook.ipynb using Jupyter Notebook or JupyterLab.
4. Click "Run All" cells. The notebook will automatically fetch the data from the web and generate all visualizations.

## 6. Product Link / Demo
* **Github**: http://github.com/Scarlett154/acc102-track-project

* **Demo**: https://video.xjtlu.edu.cn/Mediasite/MyMediasite/drafts

## 7. Limitations & Next Steps
* **Limitations**:
  * U.S.-centric dataset limits global applicability
  * 2025 snapshot may not reflect rapidly evolving skill demands
  * Self-reported salary data may contain reporting biases
  * Skills parsing from text may miss nuanced requirements

* **Next Steps**:
  * Expand analysis to include international job markets (EU, Asia-Pacific)
  * Implement temporal analysis to track skill trend evolution over 3-5 years
  * Incorporate soft skills and domain expertise in the analysis
  * Build predictive model for future skill demand forecasting
  * Develop personalized skill recommendation tool with interactive dashboard
  * Add company size and industry segmentation for deeper insights
