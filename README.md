# job_analysis

Job Market Analysis using Naukri Job Listings Dataset
Overview
This project analyzes a large dataset of job listings scraped from Naukri.com to uncover insights about hiring trends, company salaries, skills demand, and location-based job availability. The dataset includes details such as job roles, companies, experience required, salaries, locations, ratings, reviews, and responsibilities.

Dataset Description
Source: Naukri.com job listings

Size: 79,147 job entries initially

Columns:

job_id — Unique job identifier

job_role — Title of the job

company — Hiring company name

experience — Required experience range

salary — Salary details

location — Job locations

rating — Company rating

reviews — Number of company reviews

resposibilities — Job responsibilities/skills required

posted_on — Date posted (dropped during cleaning)

job_link — URL to the job posting (dropped)

company_link — URL to the company profile (dropped)

Data Cleaning
Removed rows with missing critical information (job_id, resposibilities, and company).

Filled missing values:

experience: Filled with "5-10 Yrs"

location: Filled with "Bangalore/Bengaluru"

rating: Filled with 0.0 (indicating no rating)

reviews: Filled with "0 Reviews"

Removed duplicate job entries based on job_id.

Extracted minimum and maximum experience from the experience column.

Cleaned salary data to extract minimum and maximum salaries and calculated average salary.

Converted relevant columns to proper data types.

Exploratory Data Analysis (EDA)
Top Companies by Average Salary: Identified the top 10 companies offering the highest average salaries.

Top Companies by Reviews: Visualized companies with the highest minimum number of reviews.

Popular Responsibilities: Extracted the top 10 frequently mentioned job responsibilities/skills across all listings.

Company-specific Skills: Highlighted the top responsibilities required for major companies like HDFC Bank.

Role-specific Skills: Focused on the key responsibilities for roles such as Data Analyst.

Top Hiring Locations: Identified cities with the most job postings.

Company Ratings vs Number of Jobs: Analyzed the relationship between company ratings and their hiring frequency.

Experience Distribution: Visualized the distribution of minimum experience required across jobs.

Experience vs Salary: Analyzed how average salary trends with experience.

Keyword Analysis: Created a WordCloud of the most common job responsibilities and skills.

Most In-Demand Job Roles: Listed the top 10 job roles by number of openings.

Highest Paying Job Roles: Identified the top 10 job roles by average salary.

Visualizations
Bar charts showing salary and responsibilities trends.

Pie charts highlighting company review distributions.

Scatter plots to analyze company ratings against hiring volume.

Word clouds illustrating frequent job skills.

Line plots showing experience vs salary trends.

Usage
Load the dataset using pandas.

Perform data cleaning steps to handle missing values and duplicates.

Extract and transform relevant columns (experience, salary, reviews).

Conduct exploratory analysis using pandas, seaborn, and matplotlib.

Generate visualizations for insights on the job market.

Dependencies
Python 3.x

pandas

matplotlib

seaborn

wordcloud

Install dependencies via:

pip install pandas matplotlib seaborn wordcloud
