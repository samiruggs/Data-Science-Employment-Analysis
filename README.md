# Optimizing Data Talent Acquisition, Compensation Strategy  and Scalability
### A Data-Driven Analysis of the Global Data Science Job Market using Sheets & Tableau  

---

## 📑 Table of Contents  
1. [Project Overview](#project-overview)  
2. [Data Sources](#data-sources)  
3. [Tools Used](#tools-used)  
4. [Data Cleaning & Preparation (Sheets)](#data-cleaning--preparation-sheets)  
5. [Exploratory Data Analysis (Tableau)](#exploratory-data-analysis-tableau)  
6. [Data Analysis](#data-analysis)  
7. [Results & Findings](#results--findings)  
8. [Recommendations](#recommendations)  
9. [Limitations](#limitations)  
10. [References & Links](#references--links)   

---

## 1. Project Overview  

**Stakeholder:** LifeTech Inc. *(Hypothetical Mid-Sized US Tech Company)*  

**Business Problem:**  
LifeTech is facing challenges in **hiring and retaining top data talent**. Job offers are frequently rejected, and many candidates demand salaries higher than current ranges. At the same time, the company wants to **scale operations without proportionally scaling costs**.  

**Project Goal:**  
Analyze global salary trends, job title demand, and the role of remote work using **Google Sheets for preparation** and **Tableau for visualization**. The objective is to deliver **scalable hiring insights** that balance competitiveness with cost efficiency.  

---

## 2. Data Sources  

- **Primary Dataset:** `ds_salaries.csv`  
- **Size:** 606 records, 12 columns  
- **Features:** job title, experience level, employee residence, company location, company size, salary in USD, remote ratio, employment type  
- **Timeframe:** 2020–2022  
- **Source:** [Kaggle – Data Science Job Salaries](https://www.kaggle.com/datasets/ruchi798/data-science-job-salaries)  

---

## 3. Tools Used  

- **Google Sheets** → Data cleaning, filtering, and feature creation  
- **Tableau Public** → Exploratory data analysis, interactive dashboard, visual insights  
- **GitHub** → Documentation and project repository  

---

## 4. Data Cleaning & Preparation (Sheets)  

Steps taken in Google Sheets:  

- **Removed Unnecessary Columns** → Dropped index column (`F1`)  
- **Standardized Text** → Used `=PROPER()` on job titles & experience levels to standardize text.
- I used Aliases in Tableau to change the elements of the remote ratio column from 0, 50, 100 to "Onsite", "Hybrid" and "Remote"
- I used count(ds_salaries) to ascertain the number of representations in each category

---

## 5. Exploratory Data Analysis (Tableau)

<img width="999" height="799" alt="Dashboard 1" src="https://github.com/user-attachments/assets/665becb6-5aec-45ff-a805-d7d5138fab4b" />


Interactive visualizations were built in Tableau Public to explore key aspects of the data science job market:

- **Top 5 Job Titles:** Research Scientist, Machine Learning Engineer, Data Engineer, Data Scientist, Data Analyst
- **Top 5 Employee Residences:** US, GB, CA, IN, DE
- **Employment Type:** Full-Time dominated (422/429 employees)
- **Salary by Experience Level:**
  - Entry → ~$60k
  - Intermediate → ~$93k
  - Senior → ~$133k
  - Expert → $200k+
- **Remote Work Insight:**
  - Fully Remote avg. ~$114k (highest)
  - On-Site avg. ~$103k
  - Hybrid avg. ~$74k (lowest)

📊 [View Dashboard on Tableau Public](https://public.tableau.com/views/Data_Science_Employment/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

---

### 6. Data Analysis

<img width="999" height="799" alt="Dashboard 1 (1)" src="https://github.com/user-attachments/assets/752869e9-8a21-4be0-a299-4f6dabf18222" />

 
**Salary Benchmarks (US):**
- Senior roles → $150k–$165k
- Expert-level roles → $200k+
- Entry-Role -> $90k+

**Remote Work Premium:**
- Fully Remote roles command higher pay compared to hybrid

**Job Title Salaries:**
The top 5 earners in the Job Title category are 
- Research Scientist
- Machine Learning Engineer
- Data Scientist
- Data Engineer
- Data Analyst

**Geographic Distribution:**
- US holds ~96% of employees
- UK, Canada, India, Germany are significant talent hubs

---

### 7. Results & Findings

1. **Competitive Salaries:** Senior data roles require $150k–$180k salaries to stay competitive
2. **Remote-First Norm:** Remote/hybrid hiring is now the industry standard
3. **Global Talent Availability:** Strong talent pools outside the US (UK, CA, IN, DE)
4. **Job Title Clarity:** Recognizable titles (Data Scientist, ML Engineer) improve visibility and hiring success

---

### 8. Recommendations

✅ **Revise Salary Bands** → Offer $150k–$180k for senior roles; $200k+ for expert roles  
✅ **Adopt Remote-First Hiring** → Expand hiring beyond local geographies  
✅ **Standardize Job Titles** → Use market-recognized titles (e.g., Senior Data Engineer)  
✅ **Tap Global Talent** → Pilot remote hires in UK, Canada, India and Nigeria 

---

### 9. Limitations

- Salaries are self-reported (possible bias)
- Dataset covers only 2020–2022 (market may have shifted since then)
- Currency & cost-of-living differences not accounted for
- Limited records for Expert-level roles (only 6 entries)
- Most employees that were surveyed based in the US (about 260) from a sample of 606 hence a selection bias.

---

### 10. References & Links

- **Dataset:** [Kaggle – Data Science Job Salaries](https://www.kaggle.com/datasets/ruchi798/data-science-job-salaries)
- **Tableau Dashboard:** [https://public.tableau.com/views/Data_Science_Employment/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link]
- 
📌 *This project was built using Google Sheets and Tableau, and is documented here for transparency and reproducibility.*
