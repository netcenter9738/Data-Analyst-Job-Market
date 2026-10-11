# 📊 Data Analyst Job Market Analysis: Internship Project

An Exploratory Data Analysis (EDA) of the global Data Analyst job market, focusing on geographic demand, corporate hiring trends, salary distributions, and entry-level internship opportunities. This repository contains the complete data engineering and analysis pipeline developed as part of final-year internship project.

## 📝 Project Overview
This project processes a dataset of 9,598 global Data Analyst job postings to extract quantifiable labor market insights. The primary challenge addressed is the unstructured nature of job board data—specifically messy work schedules, hidden compensation structures, and obscured corporate identities. Through programmatic data cleaning and relational merges, this analysis provides transparent benchmarks for early-career data professionals.

## 🎯 Core Technical Objectives
* **Data Standardization & Engineering:** Engineered raw text strings into binary indicator columns (e.g., `is_internship`, `is_full_time`) using iterative Python loops to enable accurate aggregation.
* **Relational Database Merging:** Executed Pandas Left Joins to map raw numerical company IDs against a corporate dimension table to reveal human-readable employer names.
* **Statistical Outlier Detection:** Applied the Interquartile Range (IQR) algorithm to identify extreme executive compensation packages, proving that the Median salary is the most robust metric for market benchmarking.
* **Early-Career Analysis:** Partitioned the dataset to evaluate the internship market, specifically analyzing remote work availability and compensation transparency for entry-level roles.

## 🛠️ Technology Stack & Dependencies
This project was developed and tested using the following specific library versions to ensure reproducibility:
* **Language:** Python 3.9+
* **Environment:** Jupyter Notebook
* **pandas** (`2.3.0`) – Data Engineering & Manipulation
* **numpy** (`2.2.6`) – Mathematical Operations & Array Management
* **matplotlib** (`3.10.3`) – Foundation Statistical Plotting
* **seaborn** (`0.13.2`) – High-Level Data Visualization

## 📁 Dataset Details
The analysis relies on two primary data files:
1. `9598_Job_postings.csv`: The primary fact table containing job titles, unstructured schedules, raw text dates, corporate requirements, and salary figures.
2. `company_dim.csv`: The dimension table acting as a dictionary to translate raw `company_id`s into actual corporate names.

## 🚀 Key Findings
1. **Geographic Centralization:** Demand remains heavily clustered in major tech hubs, requiring entry-level candidates to target localized markets.
2. **The Entry-Level Transparency Deficit:** The internship market suffers from severe compensation opacity. When disclosed, pay is overwhelmingly structured as hourly wages rather than annualized salaries.
3. **Remote Work Reality:** While senior analysts secure remote contracts, internships exhibit a strong structural bias toward on-site arrangements to facilitate live technical mentorship.
