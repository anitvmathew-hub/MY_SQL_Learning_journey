# MY_SQL_Learning_Journey


## Data

Data is a collection of facts, values, or information that can be stored and processed. Examples include employee names, salaries, customer details, product information, and transaction records.

When a large amount of data needs to be stored, organized, accessed, and managed efficiently, we use a database.

## Database

A database is an organized collection of data that allows information to be stored, retrieved, updated, and managed efficiently.

For example, an employee database may contain information such as:

Employee ID

Employee Name

Gender

Department

Job Designation

Salary

Date of Joining



* Databases make it easier to manage large amounts of structured information.

## DBMS

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

*Data storage and retrieval

*Data security

*Data modification

*User access control

*Backup and recovery

*Data integrity

## RDBMS

RDBMS (Relational Database Management System) is a type of DBMS that stores data in the form of tables consisting of rows and columns.

In an RDBMS, tables can be related to each other using keys such as Primary Keys and Foreign Keys.

Examples of RDBMS:

*MySQL

*Oracle

*PostgreSQL

*Microsoft SQL Server

*MariaDB


* RDBMS is a specialized type of DBMS designed around the relational model.

## SQL

SQL (Structured Query Language) is a standard language used to communicate with relational databases.

SQL is used to:

*Create databases and tables

*Insert data

*Retrieve data

*Update data

*Delete data

*Modify table structures

*Create relationships

*Create views

*Create procedures and functions

*Create triggers

*Control database access


Example:

SELECT *
FROM Employees;

This query retrieves all records from the Employees table.

## MySQL

MySQL is an open-source Relational Database Management System (RDBMS) that uses SQL to store, manage, and retrieve data.

MySQL is widely used for:


* Web applications
* Business applications
* Data management
* Backend development
* Reporting systems
* Data analysis



SQL is the language, while MySQL is the database management system that uses SQL.

For example:

SELECT employee_name, salary
FROM Employees
WHERE salary > 50000;

Here, SQL is the language being used, and MySQL can execute the query.

Basic Database Concepts

/*1. Database*/

A database is a container that holds related tables and other database objects.

CREATE DATABASE Employee;

To select a database:

USE Employee;

/*2. Table*/

A table stores data in rows and columns.

CREATE TABLE Employees (
    employee_id INT,
    employee_name VARCHAR(100),
    salary DECIMAL(10,2)
);

/*3. Row*/

A row represents one complete record in a table.

Example:

employee_id	employee_name	salary
101	John Smith	60000

This represents one employee record.

/*4. Column*/

A column represents a particular attribute or field.

For example:

employee_id
employee_name
salary

Each column has a specific data type.

