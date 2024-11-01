# LITA_Class_Documentation
### Project Title:The Journey of my Data Analysis

[Project Overview](#project-Overview)

Data Sources

Tools Used

Data Cleaning and preparations

[Data Analysis](#Data-Analysis)
#### Project Overview
Through my Incubator Hub experience, I aim to deepen my understanding of Excel for advanced data manipulation and visualization techniques, master SQL for efficient data querying and transformation, and become proficient in Power BI for creating interactive dashboards and insightful data visualizations.

 ### Data Sources
 The primary source of Data used here is Data sale.csv and this is an open source data that was given by the Incubator Hub.  
 
### Tools Used
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
  In the initial phase of the data claensing and preparations, we perform the following action;
  1. Data loading and inspection
  2. handling missing variables
  3. Data cleansing and formatting.
 

 ### Exploratory Data Analysis
EDA involved the exploring of the data to answer some questions about the data such as;
- what is the overall sales trend
- which product are top sellers
- what are the products on peak sales?

### Data Analysis
```
This is where we include some basic liunes of code pr queries or even some of the DAX expressions used during your analysis;

``` SQL
SELECT * FROM TABLE1
WHERE CONDITIIN = TRUE
```
### SQL create database LITA_DB
CREATE TABLE Employee (
staffid varchar(255) not null,
FirstName varchar(255) NOT NULL,
SecondName varchar (255),
Gender varchar (10),
DAate_of_Birth date,
HireDate datetime,
primary key (staffid)
)

select * from Employee
select staffid, firstname from Employee

insert into Employee (staffid,FirstName,secondname,gender,daate_of_birth,HireDate)
values( 'AB401','ayan','olakun','feale','1992-08-22','2018-02-09'),
( 'AB212', 'okorie', 'mercy', 'female','1988-10-09', '2018-10-09'),
( 'AB223', 'joshua', 'chukwuemeka', 'male','1980-10-09', '2022-02-09'),
( 'AB234', 'sanni', 'ibrahim', 'male','1958-10-09', '2019-09-23'),
( 'AB254', 'mercy', 'olanipekun', 'female','1982-10-09', '2020-02-09'),
( 'AB249', 'johnson', 'mercy', 'female','1982-10-09', '2019-12-09'),
( 'AB298', 'ayomide', 'halleluyah', 'female', '1982-10-09','2018-07-11'),
( 'AB260', 'deborah', 'justin', 'female','1982-10-09', '2018-02-09'),
( 'AB281', 'wale', 'olanipekun', 'male','1982-10-09', '2018-02-09')

----------to drop table--------
drop table employee

-----delete sql command---
delete from employee 
where staffid = 'ab281'

------truncate sql command
truncate table employee

-------identity in sql-----
CREATE TABLE PERSON (
personid int identity(1,1) primary key not null,
personname varchar (255) not null,
age int
)
insert into person (personname,age)
values ('paragon',45),
('ifenla',42),
 ('lucy',40),
 ('love',41),
 ('titi',43),
 ('peace',45),
 ('joy',49)
select* from person
--------insert more recoerds into employee table-----
insert into [dbo].[Employee]
values ( 'AB200', 'ayomide', 'halleluyah', 'female', '1982-10-09','2018-07-11'),
( 'AB405', 'deborah', 'justin', 'female','1982-10-09', '2018-02-09'),
( 'AB282', 'wale', 'olanipekun', 'male','1982-10-09', '2018-02-09'),
( 'AB278', 'shukurat', 'lasisi', 'female','1982-10-09', '2018-02-09'),
( 'AB240', 'johnson', 'mercy', 'female','1982-10-09', '2019-12-09'),
( 'AB299', 'ayomide', 'halleluyah', 'female', '1982-10-09','2018-07-11'),
( 'AB268', 'deborah', 'justin', 'female','1982-10-09', '2018-02-09'),
( 'AB286', 'wale', 'olanipekun', 'male','1982-10-09', '2018-02-09'),
( 'AB270', 'shukurat', 'lasisi', 'female','1982-10-09', '2018-02-09')
select * from employee
-----to create second table call it salvary table-----
CREATE TABLE Salvary (
salary_id int identity(1,1) not null,
staffid varchar (255),
firstname varchar(255),
lastname varchar (255),
department nvarchar(max),
salvary decimal(10,3)
)
salvary decimal(10,3)----10: precision, 3:scale
select * from salvary
-------- insert record into salvary table--------
insert into Salvary (staffid, FirstName, lastname, Department, salvary)
values ( 'AB401', 'ayan', 'olakun', 'Information Tech.', 45000.45),
( 'AB212', 'okorie', 'mercy','Account',500000.99999),
( 'AB223', 'joshua', 'chukwuemeka', 'Human Resources',100560.9339999),
( 'AB234', 'sanni', 'ibrahim', 'Sales and Marketing',845688.99),
( 'AB254', 'mercy', 'olanipekun', 'Account',8889.999999),
( 'AB249', 'johnson', 'mercy', 'Information Tech.',234000.90909090),
( 'AB298', 'ayomide', 'halleluyah', 'Logistics', 678000.991999),
( 'AB260', 'deborah', 'justin', 'Logistics',900099.00697969),
( 'AB281', 'wale', 'olanipekun', 'Information Tech',873093.2344)

insert into [dbo].[Salvary]
values ( 'AB200', 'ayomide', 'halleluyah', 'Human Resources',45699.8585),
( 'AB405', 'deborah', 'justin', 'Account',898349.900222),
( 'AB282', 'wale', 'olanipekun', 'Sales and Marketing',362636.564848),
( 'AB278', 'shukurat', 'lasisi', 'Logistics',100000.464647),
( 'AB240', 'johnson', 'mercy', 'Information Tech',3855590.9890093),
( 'AB299', 'ayomide', 'halleluyah', 'Account', 8585858.9292),
( 'AB268', 'deborah', 'justin', 'Human Resources',76767.93939)
select * from [dbo].[Salvary]
----SUM, COUNT, MAX, MIN, AVERAGE-----
SELECT SUM(salvary) from salvary
SELECT AVG(Salvary) AS AVERAGESALARY FROM Salvary
SELECT COUNT(Staffid) AS EmployeeCount FROM EMPLOYEE
SELECT COUNT(Staffid) AS NumberOfEmployee FROM Salvary

update salvary
set salvary 


--------13/09/2024---------
---update staff name-----
select * from [dbo].[Employee]
update employee
set secondname= 'Endurance'
where staffid ='AB405'
select * from [dbo].[Salvary]
update Salvary
SET department ='information tech.'
where staffid ='AB234'
update Salvary
SET department ='information tech.'
where staffid ='AB281'

SELECT * FROM Salvary
WHERE Staffid = 'AB281'

----CREATE ADDITIONAL COLUMN INTO EMPLOYEE TABLE-------
ALTER TABLE EMPLOYEE
ADD State_of_origin varchar (50) 

select * from employee
select * from employee

UPDATE EMPLOYEE
SET State_of_Origin = 'Ekiti'
where staffid = 'AB268'[Uploading SQL 1.sql…]()
SYNTAX

😆 just :

💻

to create table
|heading 1|Heading 2|Heading 3|
|---------|---------|---------|
|Table 1|Table 2|Table 3|
