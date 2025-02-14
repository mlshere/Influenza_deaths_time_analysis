# Influenza Season Analysis
*Using Data Analytics for improved staffing decisions*

## Table of Contents
1. Project Overview  
2. Objectives 
3. Data Sources 
4. Methodology  
5. Key Findings  
6. Visualizations  
7. Insights and Next Steps  
8. Repository Structure  
9. Contact

---

## Project Overview
This repository contains a data analytics project focused on **influenza trends** in the United States. The goal is to help a medical staffing agency plan for surges in patient volume during flu season by analyzing historical data on:
- Influenza-related deaths
- Population demographics
- Influenza test results

By understanding **when** and **where** demand may spike, the agency can dispatch temporary healthcare staff efficiently.

![Overview](https://github.com/user-attachments/assets/a34958f3-b9b4-442d-8ab5-c307ac5a5d8c)

---

## Objectives
- **Identify High-Risk Populations**: Examine the relationship between **elderly population (65+ years)** and **influenza-related mortality**.  
- **Determine Seasonality**: Analyze **seasonal trends** to predict peaks in influenza activity.  
- **Optimize Staffing**: Provide evidence-based recommendations to allocate medical personnel.

---

## Data Sources
1. **Influenza Deaths by Geography**  
   - **Source**: Centers for Disease Control and Prevention (CDC)  
   - **Description**: State-level counts of influenza-related deaths for multiple years.  
   - **Limitations**: Underreporting or inconsistent cause-of-death classification can skew results.    

2. **Population Data by State and Age**  
   - **Source**: US Census Bureau  
   - **Description**: Provides population estimates by state, age group, and sex.  
   - **Limitations**: Estimates may not fully account for migration or undercounting.  
     
3. **Influenza Laboratory Test Results**  
   - **Source**: CDC FluView  
   - **Description**: Survey-based weekly data on influenza test results by state.  
   - **Limitations**: Limited to reported tests; may not reflect the true total number of cases.   

---

## Methodology
1. **Data Cleaning**  
   - Removed duplicates, handled missing values, and standardized column names.  
   - Ensured consistent date formats and merged data on common state identifiers.

2. **Descriptive Analysis**  
   - Calculated **mean**, **median**, **standard deviation**, and identified potential outliers.  
   - Assessed distributions (normal vs. skewed) for mortality and population data.

3. **Correlation & Hypothesis Testing**  
   - **Pearson correlation** was used to measure relationships between elderly population (65+, 85+) and total influenza deaths.  
   - **T-tests** were conducted to check if these correlations were statistically significant.

4. **Seasonality & Forecasting**  
   - Time-series plots generated to reveal seasonal peaks in influenza cases.  
   - Basic predictive modeling (e.g., moving averages) to estimate staffing needs.

5. **Data Visualization**  
   - Developed plots and charts to communicate findings effectively.  
   - Tools: **Tableau**, **Matplotlib**, or **Seaborn** (depending on the pipeline preferences).

---

## Key Findings
- **Age Is a Key Factor**: States with higher proportions of elderly residents (65+ or 85+) experience **higher influenza-related deaths**, with correlation coefficients up to 0.95.  
- **Statistically Significant**: T-test results yield extremely small p-values (< 0.05), reinforcing that the observed correlation is not by chance.  
- **Seasonal Peaks**: Data shows consistent spikes in influenza around **late fall to early spring**, suggesting targeted staffing in Q4 and Q1 each year.

---

## Visualizations
Below are links or inline embeds to the key figures generated:


1. **State vs. Elderly Population**  
     ![State vs  elderly](https://github.com/user-attachments/assets/fc856697-dc93-4e2f-a2c3-4d8db2a51ad0)

   *Correlation between states with a high 65+ population and influenza deaths.*  

2. **Deaths per State**  
     ![Deaths per State](https://github.com/user-attachments/assets/0324098a-cee8-4024-8305-1cb935876d4d)

   *Total influenza deaths displayed by state.*  

3. **Vulnerable Population 65+**  
     ![Vulnerable population 65+](https://github.com/user-attachments/assets/d3eb6942-8f63-4310-811c-a4daf906420a)

   *Illustrates how higher concentrations of elderly residents align with higher death rates.*  

4. **Seasonality**  
      ![Seasonality](https://github.com/user-attachments/assets/7053d5a4-de06-46da-954f-5be6b518fc5b)

   *Seasonal trends in influenza mortality.*  

5. **Forecasting**  
      ![Forecasting ](https://github.com/user-attachments/assets/69ce044b-f875-4f87-a152-0f486a7d8e09)

   *Basic forecast demonstrating the expected uptick during flu season.*  

6. **Closing Thoughts**  
      ![Closing thoughts](https://github.com/user-attachments/assets/a859ecf0-f6bb-4a27-b11e-53c013f57eca)

   *Final remarks and insights for operational planning.*

---

## Insights and Next Steps
1. **Prioritize Vaccination Efforts**  
   - Focus on states with the largest elderly populations (65+).  

2. **Targeted Staffing**  
   - Deploy higher staffing levels in late autumn through spring, aligning with peak flu activity.

3. **Further Analysis**  
   - Explore **confounding variables** (e.g., vaccination rates, healthcare access, socioeconomic factors).  
   - Conduct **urban vs. rural** breakdowns and examine local hospitalization rates.

4. **Long-Term Recommendations**  
   - Develop robust **predictive models** (ARIMA, Prophet, or ML-based approaches) for future flu seasons.  
   - Integrate real-time CDC data to **dynamically adjust** staffing levels.

---

[Check out the Tableau project here.](https://public.tableau.com/app/profile/sherezade.maqueda.lafuente/viz/PreparingforInfluenzaSeason_17339958350190/Closingthoughts#2)

---

*This project is licensed under the [MIT License](./LICENSE). Feel free to explore, share, and contribute.*  

---

*© 2025 Your Name. All rights reserved.*  
