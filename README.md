# &#x20;               **Netflix User Analytics – Data Analysis Project**

# &#x20;                         **SQL • Python • Power BI**

### 

### 
NOTE : The dataset used in this project is **synthetic** and was **generated with the assistance of AI** for educational and portfolio purposes. It does **not** contain real customer or company data.

### **Project Overview**


**This project demonstrates the complete Data Analytics workflow by analyzing Netflix user behavior, subscription revenue, viewing patterns, and customer engagement.**

**The project combines SQL, Python, and Power BI to transform raw streaming data into meaningful business insights.**

**The dataset used in this project is AI-generated synthetic data designed for portfolio and educational purposes.**

### 

### Project Objectives

* Analyze Netflix user behavior.
* Measure subscription revenue and customer value.
* Identify viewing trends and content popularity.
* Discover high-value customers and regions.
* Build an interactive dashboard for business decision-making.
* Demonstrate end-to-end data analytics skills.



&#x20;Tool                               | Purpose

&#x20;---------------------------------- | ----------------------------------

&#x20;MySQL                              | Data Storage \& SQL Analysis

&#x20;Python (Pandas, NumPy, Matplotlib) | Data Cleaning, EDA \& Visualization

&#x20;Power BI                           | Interactive Dashboard

&#x20;Excel                              | Synthetic Dataset

&#x20;GitHub                             | Project Portfolio



### Dataset Information


#### Dataset Name


Netflix User Analytics

##### Rows

20,000

##### Unique Users

3,239

##### Columns

39


##### Time Period


July 2025 – July 2026


##### Dataset Includes

* User Information
* Subscription Plans
* Revenue
* Watch Time
* Content Details
* Ratings
* Devices
* Countries
* Cities
* Internet Types
* Viewing Sessions


### Project Structure
Netflix-User-Analytics/
 Dataset/
   └── Netflix\_User\_Analytics.xlsx
── SQL/
   ├── Netflix\_User\_Analytics.sql

── Python/
   └── Netflix\_User\_Analytics.ipynb

── Power BI/
   ├── Netflix Dashboard.pbix
  
── Images/
   ── Dashboard.png
   ── Revenue\_by\_Subscription\_Plan.png
   ── Revenue\_by\_Country\_Chart.png
   ── Top\_Cities\_By\_Revenue\_Chart.png
   ── Genre\_Watch\_Time.png
   ── Device\_Usage.png
   ── Monthly\_Trend.png
   ---Average\_User\_Rating.png
   ---Internet\_Connection\_Type.png
   ---Movies\_and\_TV\_Show\_Distribution.png
   ---Top\_Countries\_By\_Active\_Users.png
   ---Top\_Users.png
   ---Top\_Watched\_Titles.png
   
── README.md

── LICENSE




### SQL Analysis

The SQL portion of this project focuses on database design, querying, and business analysis.


#### SQL Topics Covered

* SELECT
* WHERE
* GROUP BY
* ORDER BY
* Aggregate Functions
* CASE Statements
* JOINS
* Views
* Stored Procedures
* User Defined Functions
* Indexes


### SQL Questions


Q1. Which subscription plan generates the highest total revenue?

Q2. Number of users in each subscription plan

Q3. Average monthly subscription fee by plan

Q4. Which content type (Movie or TV Show) is watched the most

Q5. Top 10 most watched titles

Q6. Which genres are most popular?

Q7. Which device is used the most?

Q8. Which operating system is used the most?

Q9. Which age rating has the highest average watch time?

Q10. Top 10 countries by total watch time

Q11. Which language has the highest watch time?

Q12. Which payment method is most popular?

Q13. Average completion percentage by genre

Q14. Churn risk distribution

Q15. Rank Users by Total Watch Time

Q16. Running Total Revenue by Watch Date

Q17. Categorize Users by Watch Time

Q18. Monthly Watch Time Trend

Q19. Top 3 Users in Each Country

Q20. Average Revenue Per User  by Subscription Plan

Q21. Which Titles Receive the Highest Average User Ratings?


### SQL ANSWERS

1. SELECT \*

&#x20;  FROM total\_subscription\_revenue

&#x20;  ORDER BY Total\_Revenue DESC;



2. SELECT \*

&#x20; FROM no\_of\_subscription\_users

&#x20; ORDER BY Total\_Users DESC;


3. SELECT \*

&#x20;  FROM average\_monthly\_subscription\_fee;

4. SELECT \*

&#x20; FROM content\_type\_popularity

&#x20; ORDER BY Total\_Watches DESC;


5. SELECT \*

&#x20;  FROM top\_titles

&#x20;  ORDER BY Watch\_Count DESC

&#x20;  LIMIT 10;


6\. SELECT \*

&#x20; FROM genre\_popularity

&#x20; ORDER BY Total\_Watches DESC;


7.SELECT \*

&#x20;FROM device\_usage

&#x20;ORDER BY Total\_Users DESC;


8.FROM operating\_system\_usage

&#x20;ORDER BY Total\_Users DESC;


9. SELECT \*

&#x20; FROM age\_rating\_watch\_time

&#x20; ORDER BY Avg\_Watch\_Time DESC;


10. SELECT \*

&#x20;   FROM country\_watch\_time

&#x20;   ORDER BY Total\_Watch\_Time DESC

&#x20;   LIMIT 10;



11.SELECT \*

&#x20;  FROM language\_watch\_time

&#x20;  ORDER BY Total\_Watch\_Time DESC;


12. SELECT \*

&#x20;   FROM payment\_method

&#x20;   ORDER BY Total\_Payments DESC;


13. SELECT \*

&#x20;   FROM completion\_by\_genre

&#x20;   ORDER BY Avg\_Completion DESC;


14. SELECT \*

&#x20;   FROM churn\_distribution

&#x20;   ORDER BY Total\_Users DESC;



15. SELECT \*

&#x20;   FROM rank\_users\_watch\_time

&#x20;   ORDER BY User\_Rank

&#x20;   LIMIT 10;



16. SELECT \*

&#x20;   FROM running\_revenue

&#x20;   ORDER BY Watch\_Date;



17. SELECT \*

&#x20;   FROM user\_category

&#x20;   LIMIT 20;



18. SELECT \*

&#x20;   FROM monthly\_watch\_trend

&#x20;   ORDER BY Month;



19. SELECT \*

&#x20;   FROM top3\_users\_each\_country

&#x20;   ORDER BY Country, rn;



20. SELECT \*

&#x20;   FROM avg\_Revenue\_subscription\_plan

&#x20;   ORDER BY ARPU DESC;



21. SELECT \*

&#x20;   FROM top\_rated\_titles

&#x20;   ORDER BY Average\_Rating DESC

&#x20;   LIMIT 10;



### Python Analysis


Python was used for data cleaning, exploratory data analysis (EDA), KPI calculation, and visualization.


* Data Cleaning
* Converted Date columns
* Fixed Data Types
* Removed Formatting Issues
* Checked Missing Values
* Checked Duplicate Records


### PYTHON Questions

Q1. What is the total number of unique users?

Objective: Determine the total number of unique Netflix users in the dataset.


Q2. What is the total revenue generated?

Objective: Calculate the total subscription revenue generated from all users.


Q3. What is the Average Revenue Per User (ARPU)?

Objective: Measure the average revenue generated by each unique user.


Q4. Which subscription plan generates the highest revenue?

Objective: Identify the subscription plan that contributes the most to total revenue.


Q5. Which countries contribute the most revenue?

Objective: Find the top 10 countries generating the highest subscription revenue.


Q6. Which cities generate the highest revenue?

Objective: Identify the top 10 cities contributing the highest subscription revenue.


Q7. Which genres have the highest total watch time?

Objective: Analyze which content genres generate the highest total watch time.


Q8. How does total watch time vary by month?

Objective: Analyze monthly viewing trends to identify seasonal patterns in user engagement.


Q9. What is the distribution of Movies vs TV Shows watched?

Objective: Compare user viewing preferences between Movies and TV Shows.


Q10. Which device types are most commonly used for streaming?

Objective: Identify the most popular devices used by users to stream Netflix content.


Q11. Which users spend the most time watching content?

Objective: Identify the top 10 users with the highest total watch time.


Q12. Which titles are watched the most?

Objective: Determine the top 10 most-watched movies and TV shows based on viewing sessions.


Q13. Which countries have the highest number of active users?

Objective: Identify the top 10 countries with the largest active user base.


Q14. Which genres receive the highest average user ratings?

Objective: Analyze user ratings to determine the highest-rated content genres.


Q15. Which internet connection types are most frequently used for streaming?

Objective: Analyze the distribution of internet connection types used while streaming Netflix content.


#### PYTHON Answers

1. 3,239 unique users
* Represents the full customer base included in the analysis.
* Serves as the denominator for KPIs like ARPU.


2. $21,336,179.46

* Total subscription revenue summed across all records.
* Core financial KPI for the platform.


3. $6,587.27

* Calculated as Total Revenue ÷ Total Unique Users.
* Useful for comparing value across subscription plans and segments.

4. Premium — $15,422,400.40

* Premium subscribers are the largest revenue contributor.
* Opportunity: upsell Standard/Basic users to Premium via targeted offers.

5. The top contributors (highest to lowest) are:

* &#x20;      South Korea
* &#x20;      Japan
* &#x20;      India
* &#x20;      United States
* &#x20;      Brazil
* &#x20;      Canada
* &#x20;      United Kingdom
* &#x20;      France
* &#x20;      Australia
* &#x20;      Germany

These markets should be prioritized for retention campaigns and premium upsell offers.


6. Top 10 cities generating the highest revenue (from the city revenue chart), led by major metro hubs such as

* &#x20;          Seoul
* &#x20;          Busan
* &#x20;          Incheon
* &#x20;          Daegu
* &#x20;          Sapporo
* &#x20;          Osaka
* &#x20;          Tokyo
* &#x20;          Yokohama
* &#x20;          Delhi
* &#x20;          Kolkata

These cities represent concentrated, high-value markets for marketing investment.


7.Ranked from highest to lowest total watch time:

* &#x20;                 Fantasy
* &#x20;                 Action
* &#x20;                 Adventure
* &#x20;                 Biography
* &#x20;                 Horror
* &#x20;                 Romance
* &#x20;                 Crime
* &#x20;                 Family
* &#x20;                 Animation
* &#x20;                 Documentary
* &#x20;                 Thriller
* &#x20;                 Comedy
* &#x20;                 Sci - Fi
* &#x20;                 Drama
* &#x20;                 Mystery


8. Watch time fluctuates across the year with visible peaks and troughs rather than a flat trend viewing tends to rise around certain months (consistent with holiday/vacation periods) and dip in others.

These seasonal patterns can guide content release scheduling and marketing campaign timing.


9.Movies make up the clear majority of watched content, with TV Shows representing a smaller (but still meaningful)

A balanced content library across both formats supports broader user satisfaction.


10. Mobile and Smart TV are the leading devices, followed by Laptop, Tablet, Desktop and Gaming Console

Streaming experience and app performance should be optimized first for the top devices.


11.  Top 10 Users by Total Watch Time (minutes)

Rank	User ID	Watch Time (min)

1	USR101349	2,822

2	USR102171	2,637

3	USR101133	2,546

4	USR100861	2,539

5	USR101510	2,401

6	USR102042	2,260

7	USR102720	2,176

8	USR103063	2,161

9	USR103346	2,116

10	USR103411	2,103

These are the platform's most engaged users — strong candidates for loyalty/retention programs.


12. Top 10 Most-Watched Titles (by viewing sessions)


Rank	Title	                      Views

1	Ancient Ascension	                43

2	House of Obsidian	                41

3	Sacred Ascension: Redemption    	41

4	Quiet Skyline: Redemption        	40

5	Sons of Ember	                    39

6	Sons of Ravens                   	39

7	Quiet Requiem Reborn	            39

8	Shattered Legacy Awakens	        39

9	Daughters of Wolves	              38

10	Broken Paradox: Redemption    	38





13\. Top 10 Countries by Active Users



Rank	Country	            Active Users

1	United States	             711

2	India	                     656

3	United Kingdom         	   319

4	Canada	                   271

5	France	                   248
 
6	Germany	                   240

7	Japan	                     223

8	South Korea	               197

9	Brazil	                   193

10	Australia	               181
  


14.Genres with Highest Average User Ratings


Rank	Genre	            Avg. Rating

1	Mystery	              3.88

2	Thriller	            3.87

3	Biography	            3.86

4	Action	              3.86

5	Documentary	          3.85

6	Animation	            3.84

7	Adventure	            3.84

8	Fantasy	              3.84

9	Drama	                3.83

10	Horror	            3.83

11	Romance	             3.82

12	Comedy	             3.82

13	Family	             3.82

14	Sci-Fi	             3.81

15	Crime	               3.79

Rating differences across genres are fairly narrow (3.79–3.88 on average), suggesting broadly consistent content quality/satisfaction across the catalog


15. Internet Connection Types Used for Streaming



Connection Type	   Sessions	      Share

WIFI	           8,184	          40.9%

Broadband	       5,934	           29.7%

Mobile Data	    5,882	             29.4%



* WIFI is the dominant connection type; Broadband and Mobile Data are used at nearly equal rates.
* Insights support decisions on adaptive bitrate streaming and buffering optimization across network types.


### 

### Power BI Dashboard

The Power BI dashboard provides an interactive view of Netflix's business performance.


#### KPIs

* Total Revenue
* Total Users
* ARPU
* Average Rating
* Total Watch Time


#### Dashboard Features

* Revenue by Subscription Plan
* Revenue by Country
* Monthly Watch Trend
* Device Distribution
* Genre Analysis
* Top Watched Titles
* Interactive Filters
* Drill-through Analysis


### Key Insights

* The dataset contains 20,000 streaming records from 3,239 unique users.
* Total subscription revenue exceeds $21.3 million.
* Premium subscription plans contribute significantly to total revenue.
* A small number of countries and cities generate the largest share of revenue.
* Certain genres consistently achieve higher watch time and user ratings.
* A small group of highly engaged users contributes a substantial portion of viewing activity.
* Mobile devices and Smart TVs are among the most popular streaming platforms.


### Business Recommendations

* Promote upgrades to higher-tier subscription plans.
* Invest more in high-performing genres and popular titles.
* Focus customer retention efforts on high-value users.
* Expand marketing campaigns in top revenue-generating countries and cities.
* Improve streaming performance for the most commonly used devices and internet connections.
* Use user viewing patterns to enhance personalized recommendations.


### How to Run This Project

##### SQL

1. Create the database.
2. Import the dataset.
3. Execute the SQL scripts in the following order:
* Database.sql
* Business\_Queries.sql
* Views.sql
* Stored\_Procedures.sql
* Functions.sql
* Indexes.sql


##### Python

1. Open Netflix\_User\_Analytics.ipynb.
2. Install required libraries:


&#x20;          pip install pandas numpy matplotlib openpyxl

3. Run the notebook from top to bottom.


##### Power BI

1. Open Netflix Dashboard.pbix.
2. Refresh the data source if required.
3. Explore the interactive dashboard


### 

&#x20;

### &#x20;                **👤 Author**

###### &#x20;                   **Ashutosh Jha**
                            
###### &#x20;               **Aspiring Data Analyst**

Github: https://github.com/Ashutosh-Jha07


* &#x20;     **SQL**
* &#x20;    **Python**
* &#x20;    **Power BI**
* &#x20;    **Excel**

* 
