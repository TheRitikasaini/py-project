# 📊 Overview
Ever wondered what it actually takes to land a data analyst job in India? I did too.

This project explores the Indian data job market with a focus on Data Analyst roles. Using real job posting data, I looked at which skills employers ask for the most, which ones pay the best, and most importantly which skills give you the best return on your learning investment.

The data sourced from [Luke Barousse's HF Dataset](https://huggingface.co/datasets/lukebarousse/data_jobs) which contains job titles, salaries, locations, and required skills from thousands of data related job postings.

Using Python (and an unhealthy amount of plotting), I answered some questions that every aspiring data analyst eventually asks.

>## ❓The Questions
1. What are the skills most in demand for the top 3 most popular data roles?
2. How are in-demand skills trending for Data Analysts?
3. How well do jobs and skills pay for Data Analysts?
4. What are the optimal skills for data analysts to learn? (High Demand AND High Paying) 


> ### 1. What are the most demanded skills for the top 3 most popular data roles?
First, I identified the three most common data roles and extracted their five most requested skills. The goal was simple: figure out what employers actually want instead of relying on "Top 10 Skills You MUST Learn in 2024" blog posts. 

View my notebook with detailed steps here: [2_Skill_Demand](2_Skill_Demand.ipynb).

### Results
![Likelihood of Skills Requested in Indian Job Postings](images\likelihood_of_skills_in_indian_job_postings.png)

*Bar graph visualizing the salary for the top 3 data roles and their top 5 skills associated with each.*

 ### Insights:
- Python and SQL dominate across all three data roles, making them the closest thing to non-negotiable skills.
- Cloud technologies are significantly more important for data engineers than for data analysts.
- Different roles have different priorities but SQL somehow manages to show up everywhere. It's basically the WiFi password of data jobs.

>### 2. How are in-demand skills trending for Data Analysts?
Skills change over time, so I wanted to see whether employer demand shifted throughout 2023. I grouped Data Analyst job postings by month and tracked the five most requested skills.

View my notebook: [3_Skills_Trend](3_Skills_Trend.ipynb).

### Results
![Trending Top Skills for Data Analysts in India](images\trending_top_skills_for_data_analyst_in_india.png)  
*Bar graph visualizing the trending top skills for data analysts in India in 2023.*

### Insights:
- SQL outperformed every other skill by a substantial margin, consistently maintaining a demand of around 49-55%.
- Python and Excel frequently alternated between second and third place, highlighting their complementary importance in data analysis.
- Visualization tools (Tableau and Power BI) remained less demanded than core analytical skills but showed periodic spikes, suggesting project or industry specific hiring trends.


>### 3. How well do jobs and skills pay for Data Analysts?
Everyone wants to know the salary before they learn another framework.

To answer that, I first compared salary distributions across the most common data careers in India before zooming into Data Analyst specific skills.

View my notebook: [4_Salary_Analysis](4_Salary_Analysis.ipynb).


### Results
![Salary Distributions of Data Jobs in India](images\salary_distribution_of_data_jobs_in_india.png)  
*Box plot visualizing the salary distributions for the top 6 data job titles.*

### Insights
- Machine Learning Engineers and Data Scientists generally earn the highest salaries, with wider salary ranges reflecting varying experience levels.
- Data Analysts have lower salary ranges, making them a common entry point into data careers.
- The more specialized the role, the bigger the paycheck tends to be.


>### Highest Paid & Most Demanded Skills for Data Analysts
Next, I narrowed my analysis and focused only on data analyst roles. I looked at the highest-paid skills and the most in-demand skills. I used two bar charts to showcase these.


### Results
![The Highest Paid & Most In-Demand Skills for Data Analysts in India](images\highest_paid_and_most_in_demand_skills.png)
*Two separate bar graphs visualizing the highest paid skills and most in-demand skills for data analysts in India.*

### Insights:
- Niche technologies like Dplyr, GitLab, Solidity, and Bitbucket command the highest salaries.
- Python, SQL, Tableau, and R appear in the largest number of job postings.
- High salary doesn't always mean high demand. Sometimes the highest paying skill is one you've barely heard of.

>### 4. What are the most optimal skills to learn for Data Analysts?
Learning every technology isn't realistic (unless sleep is optional).

So I calculated both median salary and job demand for each skill to identify the best skills to invest time in.

View my notebook: [5_Optimal_Skills](5_Optimal_Skills.ipynb).

### Results
![Most Optimal Skills for Data Analysts in India](images/Optimal_Skills.png)    
*A scatter plot visualizing the most optimal skills (high paying & high demand) for data analysts in India.*

### Insights:
- SQL, Excel, and Python offer the best balance of high demand and competitive salaries.
- MongoDB commands the highest median salary but has low job demand, indicating it is a niche skill with premium pay.
- Tableau, Power BI, and Spark sit nicely in the middle good salaries without being too niche.

>### Adding Techonology Categories
The previous scatter plot showed what skills performed well.

This version adds technology categories, making it much easier to spot patterns across programming languages, databases, cloud platforms, and analytics tools.

### Results
![Most Optimal Skills for Data Analysts in the India with Coloring by Technology](images/Optimal_Skills_color_coded.png)  
*A scatter plot visualizing the most optimal skills (high paying & high demand) for data analysts in the India with color labels for technology.*

### Insights:
- Programming skills (especially SQL and Python) offer the best combination of demand and salary.
- Analyst tools and databases show an interesting trade off between demand and compensation.
- Cloud and bigdata technologies provide strong complementary skills for analysts looking to branch into engineering or advanced analytics.

## 🎯 Conclusion
This project gave me a much clearer picture of what employers are actually looking for in India's data job market.

The biggest takeaway? Learn the fundamentals first. SQL and Python aren't flashy, but they consistently show up where it matters—job postings. Once those are solid, adding visualization tools, cloud technologies, or niche skills can significantly improve both career opportunities and earning potential.

The data job market isn't standing still, and neither should we. There's always another tool, another framework, or another buzzword waiting around the corner (looking at you, AI). Fortunately, the fundamentals continue to age remarkably well.

