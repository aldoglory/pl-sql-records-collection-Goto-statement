# pl-sql-records-collection-Goto-statement

 Agriculture Database – PL/SQL Project

A Demonstration of GOTO Statements, Records, and Collections in Oracle PL/SQL

 Project Overview

This project demonstrates practical applications of key PL/SQL programming concepts, including:

GOTO Statement

PL/SQL Records (User-defined & %ROWTYPE)

PL/SQL Collections (Associative Arrays, Nested Tables, Bulk Collect)

SQL DDL & DML Operations for database setup

A small agriculture database is used to simulate customers, products, and transactions.
The PL/SQL programs validate data, manipulate rows, and process in-memory collections.

 1. Database Structure
    
Database Name:

agriculture

Tables Overview

 customers
 
Column	Type	Description
customer_id	INT (PK)	Unique customer ID
cust_name	VARCHAR(50)	Customer full name
region	VARCHAR(30)	Customer region

 products
 
Column	Type	Description
product_id	INT (PK)	Unique product ID
prod_name	VARCHAR(50)	Product name
category	VARCHAR(40)	Product category

 transactions
 
Column	Type	Description
transaction_id	INT (PK)	Unique transaction ID
customer_id	INT (FK)	References customers(customer_id)
product_id	INT (FK)	References products(product_id)
sale_date	DATE	Transaction date
amount	DECIMAL(10,2)	Sale amount

 2. Sample Data Insertions

This project includes:

10 customers

10 agricultural products

10 transactions with realistic dates and amounts


 3. PL/SQL Components Demonstrated
 A. GOTO Statement

Used to:

Validate customer and product existence

Skip transaction insertion when validation fails

Jump to a labeled exit block

Demonstrates conditional control flow.

 B. Records
 
1. User-defined Record

Defines a custom structure with:

customer_id

cust_name

region

2. %ROWTYPE Record

Fetches an entire row from customers with matching structure.

 C. Collections

Includes:

1. Associative Arrays

Index-by tables for numeric data such as sales amounts.

2. Nested Tables + BULK COLLECT

Loads multiple rows into memory efficiently.



 5. Key Learning Outcomes

We  learned to:

Create and manage relational tables

Write PL/SQL blocks with validation

Use GOTO for structured control flow

Define and use custom and table-based records

Store and process multiple values using collections

Use BULK COLLECT for performance

 Tools & Technologies

Oracle Database 19c+

Oracle SQL Developer

PL/SQL

 Author

RUTERANA Gloire
Scientist & Aspiring Database Developer

📘 Assignment: PL/SQL — GOTO, Records & Collections
📅 Year: 2025
