#Artificial Intelligence and Machine Learning and Data-Related Jobs Salaries 2024

This dataset contains global information about artificial intelligence, machine learning, and data-related job salaries. It was obtained from AI Jobs and is published in the public domain under the Creative Commons CC0 license, allowing unrestricted use.

As AI and machine learning continue to transform industries, the demand for skilled professionals in these fields is growing rapidly. Roles such as Data Scientist, Research Engineer, and Machine Learning Engineer are becoming critical across sectors, from technology startups to large enterprises. I sought to analyze this dataset to uncover valuable insights into compensation trends for these roles, offering a global perspective on salary distribution across various experience levels, employment types, company sizes, and geographical locations.

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

An interactive Excel dashboard that visually represents key findings through charts and graphs. This dashboard will be designed to easily update from the source dataset, ensuring that the analysis remains current as new data becomes available.

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

## Summary statistics

- The data includes records from 2020 to 2024.

<img width="184" alt="PIVOT_1" src="https://github.com/user-attachments/assets/74215050-7db8-482e-b87d-9a61e2b40429">

The pivot table 1 displays the count of observations (data entries) for each year in the dataset, organized by the "work_year" field. Specifically, there are:

75 observations for the year 2020,
218 observations for 2021,
1,659 observations for 2022,
8,522 observations for 2023, and
43,682 observations for 2024.
In total, the dataset includes 54,156 observations.

**Average salary (in local currency) in 2024:**  $163,369 (This cannot be used for comparison between countries, except to analyze data for the same country)
**Average salary in USD in 2024:** $162,043
**Remote work ratio in 2024:** Most roles are not fully remote: 81% are neither remote nor hybrid, while 19% are fully remote.
**Salary range in USD 2024:** From $15,107 to $800,000.


