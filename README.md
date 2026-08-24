# MY_SQL_Learning_Journey

Introduction to SQL and MySQL
What is Data?

Data is a collection of facts, values, or information that can be stored and processed. Examples include employee names, salaries, customer details, product information, and transaction records.

When a large amount of data needs to be stored, organized, accessed, and managed efficiently, we use a database.

What is a Database?

A database is an organized collection of data that allows information to be stored, retrieved, updated, and managed efficiently.

For example, an employee database may contain information such as:

Employee ID
Employee Name
Gender
Department
Job Designation
Salary
Date of Joining

Databases make it easier to manage large amounts of structured information.

What is DBMS?

DBMS (Database Management System) is software used to create, store, organize, retrieve, update, and manage data in databases.

A DBMS acts as an interface between users/applications and the database.

Examples of DBMS:
MySQL
Oracle Database
Microsoft SQL Server
PostgreSQL
SQLite
Microsoft Access

A DBMS provides features such as:

Data storage and retrieval
Data security
Data modification
User access control
Backup and recovery
Data integrity
What is RDBMS?

RDBMS (Relational Database Management System) is a type of DBMS that stores data in the form of tables consisting of rows and columns.

In an RDBMS, tables can be related to each other using keys such as Primary Keys and Foreign Keys.

For example:

Employees Table
employee_id	employee_name	department_id
101	John Smith	1
102	Anita Thomas	2
Departments Table
department_id	department_name
1	Software Development
2	Marketing

Here, department_id connects the Employees table with the Departments table.

Examples of RDBMS:
MySQL
Oracle
PostgreSQL
Microsoft SQL Server
MariaDB
DBMS vs RDBMS
DBMS	RDBMS
Database Management System	Relational Database Management System
May or may not use tables	Primarily uses tables
Relationships between data may not be enforced	Relationships between tables are supported
May have less strict data integrity	Provides strong data integrity
Example: some file-based database systems	MySQL, Oracle, PostgreSQL

RDBMS is a specialized type of DBMS designed around the relational model.

What is SQL?

SQL (Structured Query Language) is a standard language used to communicate with relational databases.

SQL is used to:

Create databases and tables
Insert data
Retrieve data
Update data
Delete data
Modify table structures
Create relationships
Create views
Create procedures and functions
Create triggers
Control database access

Example:

SELECT *
FROM Employees;

This query retrieves all records from the Employees table.

What is MySQL?

MySQL is an open-source Relational Database Management System (RDBMS) that uses SQL to store, manage, and retrieve data.

MySQL is widely used for:

Web applications
Business applications
Data management
Backend development
Reporting systems
Data analysis

SQL is the language, while MySQL is the database management system that uses SQL.

For example:

SELECT employee_name, salary
FROM Employees
WHERE salary > 50000;

Here, SQL is the language being used, and MySQL can execute the query.

Basic Database Concepts
1. Database

A database is a container that holds related tables and other database objects.

CREATE DATABASE Employee;

To select a database:

USE Employee;
2. Table

A table stores data in rows and columns.

CREATE TABLE Employees (
    employee_id INT,
    employee_name VARCHAR(100),
    salary DECIMAL(10,2)
);
3. Row

A row represents one complete record in a table.

Example:

employee_id	employee_name	salary
101	John Smith	60000

This represents one employee record.

4. Column

A column represents a particular attribute or field.

For example:

employee_id
employee_name
salary

Each column has a specific data type.

SQL Data Types

Data types define what kind of data can be stored in a column.

Common MySQL Data Types
Data Type	Purpose
INT	Whole numbers
DECIMAL	Exact numeric values
VARCHAR	Variable-length text
CHAR	Fixed-length text
DATE	Date values
DATETIME	Date and time
BOOLEAN	True/False values
ENUM	One value from a predefined list

Example:

gender ENUM('M', 'F')

This allows the column to contain only the predefined values.

SQL Commands

SQL commands can be grouped into different categories.

1. DDL – Data Definition Language

DDL is used to define and modify the structure of database objects.

Common DDL commands:

CREATE
ALTER
DROP
TRUNCATE

Example:

CREATE TABLE Employees (
    employee_id INT PRIMARY KEY,
    employee_name VARCHAR(100)
);
2. DML – Data Manipulation Language

DML is used to add, modify, and remove data from tables.

Common DML commands:

INSERT
UPDATE
DELETE

Example:

INSERT INTO Employees
(employee_id, employee_name)
VALUES
(101, 'John Smith');
3. DQL – Data Query Language

DQL is used to retrieve data from a database.

The primary command is:

SELECT

Example:

SELECT employee_name, salary
FROM Employees;
4. DCL – Data Control Language

DCL is used to control access and permissions in a database.

Common commands:

GRANT
REVOKE
5. TCL – Transaction Control Language

TCL is used to manage database transactions.

Common commands:

COMMIT
ROLLBACK
SAVEPOINT

Example:

COMMIT;

This permanently saves the changes made during the transaction.
