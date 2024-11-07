# LITA_Class_Documentation
### Project Title:The Journey of my Data Analysis

[Project Overview](#project-Overview)

Data Sources

Tools Used

Data Cleaning and preparations

[Data Analysis](#Data-Analysis)
#### Project Overview
---
Through my Incubator Hub experience, I aim to deepen my understanding of Excel for advanced data manipulation and visualization techniques, master SQL for efficient data querying and transformation, and become proficient in Power BI for creating interactive dashboards and insightful data visualizations.

 ### Data Sources
 ---
 The primary source of Data used here is Data sale.csv and this is an open source data that was given by the Incubator Hub.  
 
### Tools Used
---
- Microsoft Excel is a versatile tool used for a wide range of numerical tasks, including: [Download here](https://www.microsoft.com)
  1. for Data cleaning
  2. For Data Analysis 
  3. Financial Modeling
  4. For Data Management
  5. for Data visualization.
     
- SQL - Structured Query Language SQL is a powerful language for managing and manipulating relational databases. Here are some of its key uses: [Download here](https://www.microsoft.com/en-us/sql-server/sql-server)
   1. Data Retrieval
   2. Data Manipulation
   3. Data Definition
   4. Data Control.
      
- Github is a popular platform for software development and collaboration and is also for portfolio Building. Here are some of its key uses:[Github website here](https://github.com/)
  1. Version Control
  2. Collaboration
  3. Project Management
  4. Open Source Development
  5. Learning and Experimentation.
     
- Power BI - is a powerful Business Intelligence tool used for:  [Download here](https://powerbi.microsoft.com/en-us/desktop/)
  1. Data Integration
  2. Data Transformation
  3. Data Modeling
  4. Data Visualization
  5. Data Analysis
  6. Data Storytelling.

  ### Data Cleaning and preparations
  ---
  In the initial phase of the data claensing and preparations, we perform the following action;
  1. Data loading and inspection
  2. handling missing variables
  3. Data cleansing and formatting.
 

 ### Exploratory Data Analysis
 ---
EDA involved the exploring of the data to answer some questions about the data such as;
- what is the overall sales trend
- which product are top sellers
- what are the products on peak sales?

### Data Analysis
---
This is where we include some basic lines of code or queries or even some of the DAX expressions used during your analysis;

``` SQL
create database LITA_DB

CREATE TABLE Employee (
staffid varchar (10) not null,
FirstName varchar (255) NOT NULL,
SecondName varchar (255),
Gender varchar (10),
Date_of_Birth date,
HireDate datetime,
primary key (staffid)
)
select * from Employee

insert into Employee (staffid, firstname, secondname, gender,Date_of_Birth, hiredate)
values ( 'AB401', 'ayan', 'olakun', 'female', '1992-08-22', '2018-02-09'),
( 'AB212', 'okorie', 'mercy', 'female','1988-10-09', '2018-10-09'),
( 'AB223', 'joshua', 'chukwuemeka', 'male','1980-10-09', '2022-02-09'),
( 'AB234', 'sanni', 'ibrahim', 'male','1958-10-09', '2019-09-23'),
( 'AB254', 'mercy', 'olanipekun', 'female','1982-10-09', '2020-02-09'),
( 'AB249', 'johnson', 'mercy', 'female','1982-10-09', '2019-12-09'),
( 'AB298', 'ayomide', 'halleluyah', 'female', '1982-10-09','2018-07-11'),
( 'AB260', 'deborah', 'justin', 'female','1982-10-09', '2018-02-09'),
( 'AB281', 'wale', 'olanipekun', 'male','1982-10-09', '2018-02-09')

```

### Data Visualization


😆 just :

💻

to create table
|heading 1|Heading 2|Heading 3|
|---------|---------|---------|
|Table 1|Table 2|Table 3|
