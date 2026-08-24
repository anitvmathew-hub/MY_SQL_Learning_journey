# Clauses and Joins

## Assignment Overview

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

## SQL Concepts Covered

### DISTINCT

Used to retrieve unique values from a column. In this assignment, DISTINCT is used to identify the different salary values available in the Employees table.

### Aliases (AS)

Aliases are used to provide meaningful and readable names for columns in the query output. The age and salary columns are displayed using custom aliases.

### WHERE Clause and Operators

The WHERE clause is used to filter records based on specified conditions. Queries are performed using conditions involving salary, hire date, and designation.

### UPDATE Statement

The UPDATE statement is used to modify existing records. Missing designation values are updated with Data Scientist.

### ORDER BY

Used to sort query results. Employee records are sorted by department ID in ascending order and salary in descending order.

### LIMIT

Used to restrict the number of rows returned by a query. The assignment retrieves the first five employees hired during the year 2018.

## Aggregate Functions

The following aggregate functions are used to perform calculations on employee data:

**SUM()** – Calculates the total salary.

**AVG()** – Calculates the average salary or age.

**MIN()** – Finds the minimum employee age.

**MAX()** – Finds the maximum salary.

**COUNT()** – Counts the number of employees.

## GROUP BY

Used to organize records into groups based on common values. It is used to calculate values such as the maximum salary for each location and the average salary for each designation containing the word Analyst.

## HAVING

Used to filter grouped results based on aggregate conditions. Queries identify departments with fewer than three employees and locations where female employees have an average age below 30.


## SQL Joins

**INNER JOIN**

Used to retrieve only matching records from the Employees and Departments tables. It displays employee names, designations, and their corresponding department names.

**LEFT JOIN**

Used to display all departments along with the total number of employees in each department. Departments without employees are also included in the result.

**RIGHT JOIN**

Used to display all locations along with the employees assigned to them. If a location does not have an assigned employee, the employee name is displayed as NULL.


## Objective

The objective of this assignment is to strengthen practical knowledge of SQL data querying and analysis by working with clauses, aggregate functions, grouping operations, filtering conditions, and different types of joins.
