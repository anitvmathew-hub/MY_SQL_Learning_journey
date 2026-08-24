# DDL Commands and Constraints

## Project Overview

This assignment focuses on practicing SQL data querying techniques using a relational employee database. The database consists of three related tables: Employees, Departments, and Location.

The assignment demonstrates how to retrieve and analyze data using different SQL clauses, operators, aggregate functions, grouping techniques, and joins. Various queries are performed to filter employee records, identify unique values, calculate summary statistics, sort data, and combine information from multiple tables.

## Database Tables

### 1. Employees

Stores employee-related information, including:

Employee ID
Employee Name
Gender
Age
Hire Date
Designation
Department ID
Location ID
Salary

### 2. Departments

Stores information about the different departments in the organization.

Department ID
Department Name

### 3. Location

Stores information about employee locations.

Location ID
Location Name

The tables are connected using Department ID and Location ID, which allow employee information to be related to the corresponding department and location.

### SQL Concepts Covered

#### DISTINCT

Used to retrieve unique values from a column. In this assignment, DISTINCT is used to identify the different salary values available in the Employees table.

#### Aliases (AS)

Aliases are used to provide meaningful and readable names for columns in the query output. The age and salary columns are displayed using custom aliases.

#### WHERE Clause and Operators

The WHERE clause is used to filter records based on specified conditions. Queries are performed using conditions involving salary, hire date, and designation.

#### UPDATE Statement

The UPDATE statement is used to modify existing records. Missing designation values are updated with Data Scientist.

#### ORDER BY

Used to sort query results. Employee records are sorted by department ID in ascending order and salary in descending order.

#### LIMIT

Used to restrict the number of rows returned by a query. The assignment retrieves the first five employees hired during the year 2018.

#### Aggregate Functions

The following aggregate functions are used to perform calculations on employee data:

*SUM()* – Calculates the total salary.
*AVG()* – Calculates the average salary or age.
MIN() – Finds the minimum employee age.
MAX() – Finds the maximum salary.
COUNT() – Counts the number of employees.
GROUP BY

Used to organize records into groups based on common values. It is used to calculate values such as the maximum salary for each location and the average salary for each designation containing the word Analyst.

HAVING

Used to filter grouped results based on aggregate conditions. Queries identify departments with fewer than three employees and locations where female employees have an average age below 30.

🔗 SQL Joins
INNER JOIN

Used to retrieve only matching records from the Employees and Departments tables. It displays employee names, designations, and their corresponding department names.

LEFT JOIN

Used to display all departments along with the total number of employees in each department. Departments without employees are also included in the result.

RIGHT JOIN

Used to display all locations along with the employees assigned to them. If a location does not have an assigned employee, the employee name is displayed as NULL.

🎯 Objective

The main objective of this assignment is to develop practical knowledge of querying and analyzing relational data using MySQL. It provides hands-on practice with:

Retrieving and filtering data
Using conditions and operators
Sorting and limiting query results
Applying aggregate functions
Grouping and filtering grouped data
Updating existing records
Combining related tables using different types of joins

This assignment helped strengthen my understanding of MySQL querying fundamentals and relational database operations, which are essential skills for data analysis and database management.

DDL_Commands_and_Constraints.sql
File
can you give description for readme

Absolutely. Based on your uploaded DDL Commands and Constraints assignment, here is a README description you can use for GitHub:

MySQL Assignment 1 – DDL Commands & Constraints
📌 Project Overview

This assignment focuses on practicing MySQL Data Definition Language (DDL) commands and database constraints. The goal is to understand how databases and tables are created, modified, renamed, truncated, and deleted, while also applying different constraints to maintain data accuracy and integrity.

The assignment uses an Employee database consisting of three related tables:

Employees
Departments
Location

The tables are connected using primary key and foreign key relationships.

🗂️ Database Structure
Departments Table

Stores information about different departments in the organization.

Columns:

Department ID
Department Name
Location Table

Stores information about employee locations.

Columns:

Location ID
Location Name
Employees Table

Stores employee-related information.

Columns:

Employee ID
Employee Name
Gender
Age
Hire Date
Designation
Department ID
Location ID
Salary

The department_id and location_id columns in the Employees table are connected to the Departments and Location tables using foreign key relationships.

🛠️ DDL Commands Covered
CREATE

Used to create the Employee database and the required tables, including Employees, Departments, and Location.

ALTER

Used to modify the structure of an existing table. The following operations were performed:

Added an email column to the Employees table.
Modified the size of the designation column.
Dropped the age column.
Renamed the hire_date column to date_of_joining.
RENAME

Used to rename existing tables:

Departments → Departments_Info
Location → Locations
TRUNCATE

Used to remove all records from the Employees table while keeping the table structure intact.

DROP

Used to permanently remove database objects:

Dropped the Employees table.
Dropped the Employee database.
🔒 Constraints Covered

The assignment also focuses on applying constraints to ensure data integrity and enforce valid data.

PRIMARY KEY

Used to uniquely identify each record in a table.

department_id in the Departments table
location_id in the Location table
employee_id in the Employees table
FOREIGN KEY

Used to establish relationships between tables.

department_id in Employees references the Departments table.
location_id in Employees references the Location table.
NOT NULL

Ensures that a column cannot contain a NULL value.

For example, employee names and department names are required fields.

UNIQUE

Ensures that duplicate values are not allowed in a column.

This constraint is applied to fields such as department names and location names.

AUTO_INCREMENT

Automatically generates sequential values for the location_id column when a new location is added.

ENUM

Restricts the gender column to predefined values:

M
F
CHECK

Ensures that the employee's age meets the specified condition:

CHECK (age >= 18)
DEFAULT

Automatically assigns the current date to the hire_date column if a date is not provided.

DEFAULT (CURRENT_DATE)
📊 Sample Data

Sample records were inserted into all three tables to test the table relationships, constraints, and DDL operations. The dataset includes employee details along with their corresponding departments and locations.

🎯 Objective

The main objective of this assignment is to gain practical experience with MySQL database design and table management. It demonstrates how to:

Create databases and tables
Insert sample data
Modify table structures
Rename tables and columns
Remove records using TRUNCATE
Delete tables and databases using DROP
Apply data integrity constraints
Create relationships between multiple tables using foreign keys
Use default and automatically generated values

This assignment helped strengthen my understanding of MySQL DDL commands, relational database structure, and database constraints, which are fundamental concepts for database management and data analysis.

