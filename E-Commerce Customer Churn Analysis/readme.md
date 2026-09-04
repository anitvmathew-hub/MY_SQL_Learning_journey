# E-Commerce Customer Churn Analysis using MySQL
 
## Project Overview

This project focuses on analyzing E-Commerce Customer Churn data using MySQL. The project involves creating a database and customer churn table, inserting customer data, performing data cleaning and transformation, and answering various business questions using SQL queries.

The analysis helps understand customer behavior based on factors such as:

* Customer churn status
* Tenure
* Preferred login device
* City tier
* Distance from warehouse to home
* Preferred payment mode
* Gender
* Preferred order category
* Satisfaction score
* Marital status
* Complaints
* Coupon usage
* Order count
* Cashback amount
  
## Tools Used
* MySQL
* MySQL Workbench
* SQL

## Database

The project uses the following database:

#### ecomm

The database contains the main customer churn table:

#### customer_churn

Additional table **customer_returns** is also be created for analyzing customer return information.

#### Customer Churn Table

The customer_churn table contains information such as:

* CustomerID
* Churn
* Tenure
* PreferredLoginDevice
* CityTier
* WarehouseToHome
* PreferredPaymentMode
* Gender
* HourSpendOnApp
* NumberOfDeviceRegistered
* PreferedOrderCat
* SatisfactionScore
* MaritalStatus
* NumberOfAddress
* Complain
* OrderAmountHikeFromlastYear
* CouponUsed
* OrderCount
* DaySinceLastOrder
* CashbackAmount
  
### Data Cleaning and Transformation

The project includes SQL operations for data cleaning and standardization, such as:

* Handling missing value
* Renaming columns
* Standardizing payment mode values
* Replacing inconsistent category values
* Creating new columns
* Removing unnecessary columns
* Updating data values

Examples include standardizing values such as:

* COD → Cash on Delivery
* CC → Credit Card

### Analysis Performed

The following business questions were analyzed using SQL:

1. Customer Churn Analysis<br>
  * Count of churned and active customers
  * Average tenure of churned customers
  * Total cashback amount of churned customers
  * Percentage of churned customers who complained
2. Customer Preferences<br>
  * Most preferred payment mode among active customers
  * Preferred order categories of customers using more than 5 coupons
  * Top preferred order categories based on average cashback
3. Customer Behavior<br>
  * Average number of registered devices for UPI users
  * Gender with the highest coupon usage
  * Maximum hours spent on the app by preferred order category
  * Customers with order counts above the overall average
4. Customer Satisfaction<br>
  * Average satisfaction score of customers who complained
  * Customers with the maximum satisfaction score
  * Analysis of order counts based on satisfaction scores
5. City Tier Analysis<br>
  * City tier with the highest number of customers
  * Churned customers based on city tier and preferred order category
6. Distance Analysis<br>

  Customers were categorized based on their distance from the warehouse:

  Distance	Category:<br>
<= 5 km	Very Close Distance<br>
<= 10 km	Close Distance<br>
<= 15 km	Moderate Distance<br> >5 km	Far Distance

The churn status breakdown was then analyzed for each distance category.

### SQL Concepts Used

This project demonstrates the use of:

* SELECT
* WHERE
* GROUP BY
* ORDER BY
* HAVING
* LIMIT
* DISTINCT
* COUNT()
* SUM()
* AVG()
* MAX()
* ROUND()
* CASE
* Subqueries
* INNER JOIN

  
### Customer Returns Analysis

A customer_returns table was created to store customer return details.<br>

The table contains:

* ReturnID
* CustomerID
* ReturnDate
* RefundAmount

SQL joins were used to combine customer return information with customer churn data.<br>

Analysis performed:

* Display return details along with customer information
* Identify customers who have churned
* Identify customers who have made complaints

Through this project, I gained hands-on experience in:

* Database creation and management
* Creating tables and inserting data
* Data cleaning using SQL
* Aggregate functions
* Filtering and grouping data
* Using CASE statements for categorization
* Writing subqueries
* Performing joins between tables
* Solving real-world business questions using SQL
