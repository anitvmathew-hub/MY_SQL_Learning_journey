# DDL Commands and Constraints


## Assignment Overview

This assignment focuses on practicing MySQL Data Definition Language (DDL) commands and database constraints. The goal is to understand how databases and tables are created, modified, renamed, truncated, and deleted, while also applying different constraints to maintain data accuracy and integrity.

The assignment uses an Employee database consisting of three related tables:

Employees

Departments

Location

The tables are connected using primary key and foreign key relationships.

## Database Structure

### Departments Table

Stores information about different departments in the organization.

#### Columns:

Department ID

Department Name

### Location Table

Stores information about employee locations.

#### Columns:

Location ID

Location Name

### Employees Table

Stores employee-related information.

#### Columns:

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

## DDL Commands Covered

#### CREATE

Used to create the Employee database and the required tables, including Employees, Departments, and Location.

#### ALTER

Used to modify the structure of an existing table. The following operations were performed:


Added an email column to the Employees table.

Modified the size of the designation column.

Dropped the age column.

Renamed the hire_date column to date_of_joining.

#### RENAME

Used to rename existing tables:

Departments → Departments_Info
Location → Locations

#### TRUNCATE

Used to remove all records from the Employees table while keeping the table structure intact.

#### DROP

Used to permanently remove database objects:

Dropped the Employees table.
Dropped the Employee database.

## Constraints Covered

The assignment also focuses on applying constraints to ensure data integrity and enforce valid data.

#### PRIMARY KEY

Used to uniquely identify each record in a table.

department_id in the Departments table
location_id in the Location table
employee_id in the Employees table

#### FOREIGN KEY

Used to establish relationships between tables.

department_id in Employees references the Departments table.
location_id in Employees references the Location table.

#### NOT NULL

Ensures that a column cannot contain a NULL value.

For example, employee names and department names are required fields.

#### UNIQUE

Ensures that duplicate values are not allowed in a column.

This constraint is applied to fields such as department names and location names.

#### AUTO_INCREMENT

Automatically generates sequential values for the location_id column when a new location is added.


#### CHECK
Ensures that the employee's age meets the specified condition:

CHECK (age >= 18)

#### DEFAULT

Automatically assigns the current date to the hire_date column if a date is not provided.

DEFAULT (CURRENT_DATE)


## ENUM

Restricts the gender column to predefined values:

M

F

## Sample Data

Sample records were inserted into all three tables to test the table relationships, constraints, and DDL operations. The dataset includes employee details along with their corresponding departments and locations.

## Conclusion

This assignment helped strengthen my understanding of MySQL DDL commands, relational database structure, and database constraints, which are fundamental concepts for database management and data analysis.

