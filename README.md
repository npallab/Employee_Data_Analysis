
# Data Analysis of Employees from Scrapped Data
1. Project Overview : This project aims to leverage SQL to analyze employee-related data, focusing on training, development, and engagement. The goal is to derive actionable insights that can inform decision-making and improve organizational performance.








## Data Description


1. EMPLOYEES: Contains employee details

```bash

create or replace TABLE SQL_PROJECT.PUBLIC.EMPLOYEES (
    EMPID NUMBER(38,0) NOT NULL,
    FIRSTNAME VARCHAR(100),
    LASTNAME VARCHAR(100),
    STARTDATE DATE,
    EXITDATE DATE,
    TITLE VARCHAR(100),
    SUPERVISOR VARCHAR(200),
    ADEMAIL VARCHAR(100),
    BUSINESSUNIT VARCHAR(100),
    EMPLOYEESTATUS VARCHAR(50),
    EMPLOYEETYPE VARCHAR(50),
    PAYZONE VARCHAR(50),
    EMPLOYEECLASSIFICATIONTYPE VARCHAR(100),
    TERMINATIONTYPE VARCHAR(50),
    TERMINATIONDESCRIPTION VARCHAR(100),
    DEPARTMENTTYPE VARCHAR(100),
    DIVISION VARCHAR(100),
    DOB VARCHAR(20),
    STATE VARCHAR(50),
    JOBFUNCTIONDESCRIPTION VARCHAR(100),
    GENDERCODE VARCHAR(20),
    LOCATIONCODE VARCHAR(50),
    RACEDESC VARCHAR(50),
    MARITALDESC VARCHAR(50),
    PERFORMANCESCORE VARCHAR(50),
    EMPLOYEERATING VARCHAR(50),
    primary key (EMPID)
);

```
2. TRAINING_DEV: Records details of employee training programs.

```bash

create or replace TABLE SQL_PROJECT.PUBLIC.TRAINING_DEV (
    EMPLOYEE_ID NUMBER(38,0) NOT NULL,
    TRAINING_DATE DATE NOT NULL,
    TRAINING_PROGRAM_NAME VARCHAR(100) NOT NULL,
    TRAINING_TYPE VARCHAR(50),
    TRAINING_OUTCOME VARCHAR(50),
    LOCATION VARCHAR(100),
    TRAINER VARCHAR(100),
    TRAINING_DURATION NUMBER(38,0),
    TRAINING_COST NUMBER(10,2),
    primary key (EMPLOYEE_ID, TRAINING_DATE, TRAINING_PROGRAM_NAME)
);


```

3. EMPLOYEE_ENGAGEMENT_SURVEY: Records details of employee training programs.

```bash

create or replace TABLE SQL_PROJECT.PUBLIC.EMPLOYEE_ENGAGEMENT_SURVEY (
    EMPLOYEE_ID NUMBER(38,0) NOT NULL,
    SURVEY_DATE VARCHAR(20) NOT NULL,
    ENGAGEMENT_SCORE NUMBER(5,2),
    SATISFACTION_SCORE NUMBER(5,2),
    WORK_LIFE_BALANCE_SCORE NUMBER(5,2),
    primary key (EMPLOYEE_ID, SURVEY_DATE)
);



```


## Following Business Queries are included here in 

1.What is the average engagement score across different departments?

2.How does training impact employee performance and retention?

3.What are the common reasons for employee termination?

4.How do demographic factors (e.g., gender, race, marital status) correlate with employee satisfaction and performance?

5.Which training programs have the highest impact on performance improvement?

6.What is the distribution of employee ratings across different business units?

7.How does employee engagement vary by job function?

8.What is the correlation between employee age and job satisfaction?

9.What is the average training cost per department?

10.What is the trend of employee retention over time?


## Dashboard

Dashboard Link(may not be operational) : https://lookerstudio.google.com/reporting/2831e881-90e0-4287-8c10-537ff6706964



## Screenshots

[Dashboard Screenshot]

<a href="https://ibb.co/vZ1tKsy"><img src="https://i.ibb.co/4PWQ5sv/Screenshot-2024-07-15-at-2-01-47-PM.png" alt="Screenshot-2024-07-15-at-2-01-47-PM" border="0" /></a>

## Authors

- [@npallab](https://www.github.com/npallab)


## 🚀 About Me
I am a Risk Analytics Professional with : Certififcation in Machine Learning from IIT Roorkee, Certified Scrum Master, Black Belt in Six Six Sigma, PMP Trained. I have worked with Amazon in the past and currently working as a Senior Analyst in Payment Risk team in Airbnb.


## 🔗 Links

[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/pallabnath/)


## 🛠 Skills
SQL,Python,C/C++,Machine Learning, Data Analytics, Project Management, Consulting, Risk Management


## Tech Stack

**Data Warehouse** Snowflake

**Language** MYSQL

**Data Source** Kaggle

