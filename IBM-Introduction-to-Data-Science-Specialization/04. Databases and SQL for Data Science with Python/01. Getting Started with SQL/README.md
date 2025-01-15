# Week01 - Getting Started with SQL

SQL is a powerful language that's used for communicating with databases.

## Welcome to SQL for Data Science

## Why SQL for Data Science?

- big data
- table with a few rows
- small start up
- big database
- mobile phone

## What will we learn in the course?

- basics for SQL and relational databases
- working knowledge of SQL and databases
- connect to database and run SQL queries
- python and Jupyter notebooks to analyze data
- assignment to apply concepts with real word dataset

## Course overview

- basic of SQL
- relational database model
- At the end of the course, you will be able to discussSQL basics and explain aspects of the relational database model
- At the end of the lesson, you will be able to:
    - describe SQL, data, database, relational database
    - list five SQL commands

## Introduction to Databases

## What is SQL?

SQL (Structured Query Language) is a language used for relational databases to query or get data out of a database.

## What is data?

Data is a collection of facts in the form of words, numbers, or even pictures. Data is one of the most critical assets of any business.

## What is a database?

- A database is a repository of data.
- A program stores data.
- A database also provides the functionality for adding, modifying, and querying that data.

## Type of database:

1. non-relational database
2. relational database:
    - data store in tabular form - with columns and rows
    - relationships can exist between tables

## DBMS (Database Management System):

- database: repository of data
- DBMS (Database management System): a software to manage the databases
- RDBMS - Relational database management system: a set of software tools that controls data
    - access, organization, and storage
- Example:
    - MySQL, Oracle Database, IBM DB2, and DB2 warehouse

## 5 simple commands in SQL:

1. `Create`: create a table
2. `Insert`: insert data to populate the table
3. `Select`: select data from the table
4. `Update`: update data in the table
5. `Delete`: delete data from the table.

## SELECT statement

- learning object: retrieving data from a table
- Common SQL command structure

```sql
SELECT column1, column2, ...
FROM table_name
WHERE condition
;
```

- The main purpose of a database management system, is not just to store the data but also facilitate retrieval of the data.
    - select statement: query
    - results from the query: Results set/table

```sql
select * from <tableName>
```

- select some columns

```sql
SELECT book_id, title from Book
WHERE book_id = "B1"
```

## COUNT, DISTINCT, LIMIT

- `count`: a built-in database function that retrieves the number of rows that match the query criteria.
    - Number of rows in a table
        
        ```sql
        select COUNT(*) from tableName
        ```
        
    - Rows in the MEDALS table where Country is Canada
        
        ```sql
        select COUNT(COUNTRY) from MEDALS
        	where COUNTRY = "CANADA"
        ```
        
- `DISTINCT`: is used to remove duplicate values from a results set.
    - Retrieve unique values in a column
        
        ```sql
        select DISTINCT columnName from tableName
        ```
        
    - List of unique countries that received GOLD medals:
        
        ```sql
        select DISTINCT COUNTRY from MEDALS
        		where MEDALTYPE = "GOLD"
        ```
        
- `LIMIT`: is used for restricting the number of rows retrieved from the database.
    - retrieve just the first 10 rows in a table
        
        ```sql
        select * from tableName LIMIT 10
        ```
        
    - retrieve 5 rows in the MEDALS table for a particular year
    
    ```sql
    select * from MEDALS
    where YEAR = 2018 LIMIT 5
    ```
    

## **INSERT Statement**

- DML statement: Data Manipulation Language (DML) statement used to read and modify data.
- `INSERT` statement: to add the data to the table

```sql
INSERT  INTO TableName
	<(ColumnName, ... )>
VALUES(Value, ... )
```

- E.g.

```sql
INSERT INTO AUTHOR
	(AUTHO_ID, LASTNAME, FIRSTNAME, EMAIL, CITY, COUNTRY)
VLAUES("A1","Chong","Raul","rfc@ibm.com","Toronto","CA")
```

- insert multiple rows

```sql
INSERT INTO AUTHOR
	(AUTHO_ID, LASTNAME, FIRSTNAME, EMAIL, CITY, COUNTRY)
VLAUES
	("A1","Chong","Raul","rfc@ibm.com","Toronto","CA")
	("A2","Ahuja","Rav","ra@ibm.com","Toronto","CA")
```

## **UPDATE and DELETE Statements**

### UPDATE

After a table is created and populated with data, the data in a table can be altered with the `UPDATE` statement.

The `UPDATE` statement is one of the data manipulation language or DML statements. DML statements are used to read and modify data.

The `UPDATE` statement should be like:

```sql
UPDATE TableName
SET [[ColumnName] = [Value]]
<WHERE [Condition]>
```

- E.g.
    ![Untitled](https://user-images.githubusercontent.com/52702712/203136630-a4964131-4a80-4183-8fb6-8e23af85881a.png)

    

```sql
UPDATE AUTHOR
SET LASTNAME = "KATTA"
	LASTNAME = "LAKSHMI"
WHERE AUTHOR_ID = "A2"
```

### DELETE

- To remove 1 or more rows from the table
- The `DELETE` statement is one of the data manipulation language or DML statements. DML statements are used to read and modify data.
- E.g.

![Untitled 1](https://user-images.githubusercontent.com/52702712/203136691-1f820670-52f9-49ed-96da-e93b2707d7da.png)


```sql
DELETE FROM AUTHOR
	WHERE AUTHOR_ID IN ('A2','A3')
```

## Summary & Highlights

 After this session, you should know:

- You can use Data Manipulation Language (DML) statements to read and modify data.
- The search condition of the WHERE clause uses a predicate to refine the search.
- COUNT, DISTINCT, and LIMIT are expressions that are used with SELECT statements.
- INSERT, UPDATE, and DELETE are DML statements for populating and changing tables.
