# Optimizing Data Talent Acquisition and Compensation Strategy  
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
**Stakeholder:** A mid-sized technology company (hypothetical).  

**Business Problem:**  
The company I call ‘LifeTech Inc.’ struggles to attract and retain top data professionals. Job offers are frequently rejected, and leadership suspects their salary and remote work policies are not aligned with market standards.  

**Goal:**  
Analyze global salary trends, job demand, and the impact of remote work using a real-world dataset. Provide actionable recommendations for competitive compensation and hiring strategies.  

---

## 2. Data Sources  
- **Primary Dataset:** Data Science Job Salaries (2020–2022)  
- **Records:** 606 rows  
- **Features:** 12 columns (job title, experience level, salary in USD, company location, employee residence, company size, remote ratio, employment type, etc.)  
- **Source:** [Kaggle – Data Science Job Salaries](https://www.kaggle.com/datasets/ruchi798/data-science-job-salaries)  

---

## 3. Tools Used  
- **Google Sheets** → Data cleaning, preparation, feature engineering  
- **Tableau Public** → Exploratory analysis & interactive dashboard  
- **GitHub** → Documentation, dataset storage, and sharing dashboard links  

---

## 4. Data Cleaning & Preparation (Sheets)  
Steps taken in Google Sheets:  

1. **Removed unnecessary column**  
   - Dropped index column `F1`  
2. **Standardized text**  
   - Used `=PROPER()` to ensure consistent formatting for job titles and experience levels  
3. **Created new feature: Remote Work Type**  
   ```excel
   =IFS(C2=0,"On-Site",C2=50,"Hybrid",C2=100,"Fully Remote")

## 5. Exploratory Data Analysis (Tableau)

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

**Salary Benchmarks (US):**
- Senior roles → $150k–$165k
- Expert-level roles → $200k+
- Entry-Role -> $80k+

**Remote Work Premium:**
- Fully Remote roles command higher pay compared to hybrid

**Job Title Salaries:**
The top 5 earners in the Job Title category are 
- Research Scientist
- Machine Learning Engineer
- Data Engineer salaries
- Data Scientist
- Data Analyst

**Geographic Distribution:**
- US holds ~70% of employees
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
✅ **Tap Global Talent** → Pilot remote hires in UK, Canada, India  

---

### 9. Limitations

- Salaries are self-reported (possible bias)
- Dataset covers only 2020–2022 (market may have shifted since then)
- Currency & cost-of-living differences not accounted for
- Limited records for Expert-level roles (only 6 entries)

---

### 10. References & Links

- **Dataset:** [Kaggle – Data Science Job Salaries](https://www.kaggle.com/datasets/ruchi798/data-science-job-salaries)
- **Tableau Dashboard:** [Insert your Tableau Public link here]
- 
📌 *This project was built using Google Sheets and Tableau, and is documented here for transparency and reproducibility.*
