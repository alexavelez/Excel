# Artificial Intelligence and Machine Learning and Data-Related Jobs Salaries 2024

This dataset contains global information about artificial intelligence, machine learning, and data-related job salaries. It was obtained from AI Jobs and is published in the public domain under the Creative Commons CC0 license, allowing unrestricted use.

As AI and machine learning continue transforming industries, the demand for skilled professionals in these fields is growing rapidly. Roles such as Data Scientist, Research Engineer, and Machine Learning Engineer are becoming critical across sectors, from technology startups to large enterprises. I sought to analyze this dataset to uncover valuable insights into compensation trends for these roles, offering a global perspective on salary distribution across various experience levels, employment types, company sizes, and geographical locations.

Understanding salary trends is essential for both employers and professionals as they navigate a competitive landscape. For job seekers, this data provides insight into how factors such as experience, remote work, and company size influence salaries. For employers, it serves as a benchmark for attracting and retaining top talent in this evolving field.

## The questions I aim to answer with this dataset are:
* What is the average salary for different roles (e.g., Data Scientist, Research Engineer) across various experience levels?
* How does the remote work ratio affect salaries across different regions or job roles?
* How do salaries differ across regions (employee residence vs. company location)?
* What is the average salary based on different employment types (full-time, part-time, contract)?
* How does company size influence salaries across job titles or experience levels?

I will answer these questions for the year 2024 and compare them with previous years.

## Deliverables:
As part of this analysis, the following deliverables will be provided:

Excel Analysis:

A comprehensive analysis using pivot tables to summarize key salary trends. The pivot tables will allow for filtering and exploring salary data across different job titles, experience levels, regions, and employment types.

Dynamic Dashboard:

An interactive Excel dashboard that visually represents key findings through charts and graphs.

## The dataset

The dataset contains a single table with all salary information structured as follows:

**work_year** The year the salary was paid.  

**experience_level** The experience level in the job during the year with the following possible values:  
EN: Entry-level / Junior  
MI: Mid-level / Intermediate
SE: Senior-level / Expert  
EX: Executive-level / Director  

**employment_type** The type of employment for the role:
PT:Part-time  
FT:Full-time
CT: Contract
FL: Freelance  

**job_title** The role worked in during the year.  

**salary** The total gross salary amount paid.  

**salary_currency** The currency of the salary paid as an ISO 4217 currency code.  

**salary_in_usd** The salary in USD (FX rate divided by avg. USD rate of respective year) via statistical data from the BIS and central banks.  

**employee_residence** Employee's primary country of residence in during the work year as an ISO 3166 country code.  

**remote_ratio** The overall amount of work done remotely, possible values are as follows:
0: No remote work (less than 20%)
50: Partially remote/hybird
100 :Fully remote (more than 80%)  

**company_location** The country of the employer's main office or contracting branch as an ISO 3166 country code.  

**company_size** The average number of people that worked for the company during the year:
S: less than 50 employees (small)
M: 50 to 250 employees (medium)
L :more than 250 employees (large)

### Missing Values
There are no missing values in the dataset.

### Data Preparation
All the columns are ready for analysis except for the job_title column. The job_title column contains 252 unique job titles. Some titles refer to the same role but are expressed with different wording or abbreviations. For instance, roles like "Business Intelligence Data Analyst," "BI Analyst," and "Business Intelligence Analyst," all describe the same type of job but are written with slight variations. Moreover, there is overlap between many of the roles. 

To ensure consistency in the analyses, these titles need to be standardized or grouped into common categories. For this analysis, I opted for groping them into the following categories:

- Data Analysis
- Data Science
- Data Engineering
- Data Management
- Business Intelligence
- Machine Learning
- Software & Cloud Engineering
- Product & Project Management
- Research & Specialized Roles
- General & Other Roles

To achieve this, I created a new column named job_category and a lookup table in a separate sheet named job_category_lookup. This allows for changes to the category assigned to job titles in the future if needed. 

## Summary statistics

The data includes records from 2020 to 2024. The pivot table 1 displays the count of observations (data entries) for each year in the dataset, organized by the "work_year" field. Specifically, there are:

<img width="272" alt="Pivot1" src="https://github.com/user-attachments/assets/50549cf2-54db-4b86-8a61-a3de03575daa">  


75 observations for the year 2020,
218 observations for 2021,
1,659 (3%) observations for 2022,
8,522 (16%) observations for 2023, and
43,682 (81%) observations for 2024.
In total, the dataset includes 54,156 observations.

Table 1 presents the summary statistics of salaries from 2020 to 2024, providing insights into key metrics such as the average, median, minimum, and maximum salaries for each year. This data allows for a comparison of salary trends across different years.

<img width="718" alt="table_1" src="https://github.com/user-attachments/assets/597ac082-7018-47b6-814f-cbb8f00d0877">  


**Average salary (in local currency) in 2024:**  $163,369 (This cannot be used for comparison between countries, except to analyze data for the same country)  

**Average salary in USD in 2024:** $162,043  

**Remote work ratio in 2024:** Most roles are not fully remote: 81% are neither remote nor hybrid, while 19% are fully remote.  The pivot table 2 shows the remote work ratio by year from 2020 to 2024.

**Salary range in USD 2024:** From $15,107 to $800,000.  

## Job Title Distribution

The top 5 job titles:

- Data Scientist:	92 records
- Data Engineer:	91 records
- Data Analyst:	90 records
- Software Engineer:	89 records
- Machine Learning Engineer: 88 records

However, as discussed earlier, this list doesn't show the full picture, as other similar roles also fall under the title "Data Scientist," such as Data Scientist Lead, Decision Scientist, Lead Data Scientist, Applied Data Scientist, Principal Data Scientist, etc.

The pivot table 3 shows Job Category Distribution with Percentage of Total. Grouped by category, the top 5 job roles are:

<img width="373" alt="pivot3" src="https://github.com/user-attachments/assets/48f3e26f-b195-44f1-b68f-fab7c6abcced">  


## Experience Level Distribution

Senior (SE): 32,206 (59.5%) records
Mid-level (MI): 15,872 (29.3%) records
Entry-level (EN): 4,908 (9.1%) records
Executive (EX): 1,170 (2.1%)records

## Employment Type Distribution:

Full-time (FT): 53,953 records (99.62%)
Part-time (PT), Contract (CT), and Freelance (FL) roles are much fewer in number (0.38%).

## Company Location Distribution:

The dataset contains companies from 82 different countries; however, the vast majority are based in the US, which accounts for 93.46% of the total. The Pivot Table 6 shows the distribution of top 5 countries by company location.

<img width="450" alt="pivot 6" src="https://github.com/user-attachments/assets/39a5f921-5de4-40e4-becf-e176206419d4">

## Distribution of Employee Country of Residence 

The dataset contains 91 unique countries of residence for employees, while company locations are distributed across 82 countries. Despite the wider range of employee residences, the top 5 countries of residence closely mirror the top 5 company locations. The majority of employees reside in the US, representing 93.20%, followed by Canada (3.20%), Great Britain (2.96%), Germany (0.33%), and Spain (0.31%). This strong alignment suggests that, in most cases, employees are likely working in the same country where they reside, although the presence of remote work across borders cannot be completely ruled out.

The Pivot Table 7 shows the top 5 countries by employee residence 

<img width="305" alt="pivot7" src="https://github.com/user-attachments/assets/7f22fa59-681b-4f0c-97f0-ae97081cf3d9">

Rate of remote ratio decreasing



