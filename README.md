
# My Learning Journey with DSA - Mastering SQL

I am excited to share my journey with Digital SkillUp Africa (DSA), the incubator hub. This repository is a documentation of my progress in SQL, understanding and demonstrating real-world tasks, problem-solving, and data-driven decision-making.

### What is SQL?

SQL stands for Structure Query Language. It is used to store, retrieve and manage data in relational databases. 

### Basic SQL Commands


SQL commands are instructions. It is used to communicate with the database. It is also used to perform specific tasks, functions, and queries of data.

### *Types of SQL Commands*

-*DDL (Data Definition Language)*: Create, Alter, Drop, Truncate - define your structure!


-*DML (Data Manipulation Language)*: Insert, Merge, Update or Delete your data!

-*DCL (Data Control Language)*:  Grant, revoke -  Secure your data with permission!


-*TCL (Transaction Control Language)*: Commit, Rollback - control your database transaction!

-*DQL (Data Query Language)*: Select - fetch and analyse your data smartly!

### *SQL Queries*


### *Query Examples*
```
-- Alter table to add new column
ALTER TABLE EMPLOYEE ADD [State of Origin] varchar(100);

-- Alter column data type
ALTER TABLE Salary ALTER COLUMN Salary Decimal(10,3);

-- Update department
UPDATE Salary SET Department = 'Information Tech' WHERE Staffid IN ('AB401', 'AB249');
```

*Business Questions*
1. *Total number of staff*
```
SELECT Count(Distinct Staffid) AS TotalEmployee FROM Employee;
```

2. *Calculate total number of staff from each state*
```
SELECT [STATE OF ORIGIN], Count(Distinct Staffid) AS TotalEmployee 
FROM EMPLOYEE 
GROUP BY [STATE OF ORIGIN] 
ORDER BY TotalEmployee ASC;
```

3. *Calculate total number of staff from each department*
```
SELECT Department, Count(Distinct Staffid) AS TotalEmployee 
FROM Salary 
GROUP BY Department 
ORDER BY TotalEmployee DESC;
```

4. *Find those that earn above 500,000 salary*
```
SELECT * FROM Salary WHERE Salary > 500000;
```

5. *Find those that earn below 500,000 salary*
```
SELECT * FROM Salary WHERE Salary < 500000;
```

*Tools Used*


- *SQL Server* as Database
- *SSMS (SQL Server Management Studio)* for Query Execution

SQL is more than just a query language; it's a powerful tool for transforming data into decisions.
