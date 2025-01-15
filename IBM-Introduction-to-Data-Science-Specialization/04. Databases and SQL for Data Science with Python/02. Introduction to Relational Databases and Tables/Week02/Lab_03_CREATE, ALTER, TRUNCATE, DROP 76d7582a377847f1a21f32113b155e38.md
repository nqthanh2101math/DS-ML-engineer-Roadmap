# Lab_03_CREATE, ALTER, TRUNCATE, DROP

![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/IDSNlogo.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/IDSNlogo.png)

# **Hands-on Lab : CREATE, ALTER, TRUNCATE, DROP**

**Estimated time needed:** 15 minutes

In this lab, you will learn some commonly used DDL (Data Definition Language) statements of SQL. First you will learn the CREATE statement, which is used to create a new table in a database. Next, you will learn the ALTER statement which is used to add, delete, or modify columns in an existing table. Then, you will learn the TRUNCATE statement which is used to remove all rows from an existing table without deleting the table itself. Lastly, you will learn the DROP statement which is used to delete an existing table in a database.

**How does the syntax of a CREATE statement look?**

```sql

CREATE TABLE table_name (
    column1 datatype,
    column2 datatype,
    column3 datatype,
   ....
);

```

**How does the syntax of an ALTER statement look?**

```sql

ALTERTABLE table_name
ADDCOLUMN column_name data_type column_constraint;

ALTERTABLE table_name
DROPCOLUMN column_name;

ALTERTABLE table_name
ALTERCOLUMN column_nameSET DATATYPE data_type;

ALTERTABLE table_name
RENAMECOLUMN current_column_nameTO new_column_name;

```

**How does the syntax of a TRUNCATE statement look?**

```sql

TRUNCATETABLE table_name;

```

**How does the syntax of a DROP statement look?**

```sql

DROPTABLE table_name;

```

## **Software Used in this Lab**

In this lab, you will use [IBM Db2 Database](https://www.ibm.com/products/db2-database?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork22-2022-01-01). Db2 is a Relational Database Management System (RDBMS) from IBM, designed to store, analyze and retrieve the data efficiently.

To complete this lab you will utilize a Db2 database service on IBM Cloud. If you did not already complete this lab task earlier in this module, you will not yet have access to Db2 on IBM Cloud, and you will need to follow this lab first:

- [Hands-on Lab : Sign up for IBM Cloud, Create Db2 service instance and Get started with the Db2 console](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20Sign%20up%20for%20IBM%20Cloud%20-%20Create%20Db2%20service%20instance%20-%20Get%20started%20with%20the%20Db2%20console/instructional-labs.md.html)

## **Database Used in this Lab**

The databases used in this lab are internal databases.

## **Objectives**

After completing this lab, you will be able to:

- Create a new table in a database
- Add, delete, or modify columns in an existing table
- Remove all rows from an existing table without deleting the table itself
- Delete an existing table in a database

## **Instructions**

When you approach the exercises in this lab, follow the instructions to run the queries on Db2:

- Go to the [Resource List](https://cloud.ibm.com/resources?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork22-2022-01-01) of IBM Cloud by logging in where you can find the Db2 service instance that you created in a previous lab under **Services** section. Click on the **Db2-xx service**. Next, open the Db2 Console by clicking on **Open Console** button. Click on the 3-bar menu icon in the top left corner and go to the **Run SQL** page. The Run SQL tool enables you to run SQL statements.
    - If needed, follow [Hands-on Lab : Sign up for IBM Cloud, Create Db2 service instance and Get started with the Db2 console](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20Sign%20up%20for%20IBM%20Cloud%20-%20Create%20Db2%20service%20instance%20-%20Get%20started%20with%20the%20Db2%20console/instructional-labs.md.html)

# **Exercise 1: CREATE**

In this exercise, you will use the CREATE statement to create two new tables using Db2.

1. You need to create two tables, **PETSALE** and **PET**. To create the two tables PETSALE and PET, copy the code below and paste it to the textbox of the **Run SQL** page. Click **Run all**.
    
    ```sql
    
    CREATETABLE PETSALE (
        ID INTEGERNOTNULL,
        PET CHAR(20),
        SALEPRICE DECIMAL(6,2),
        PROFIT DECIMAL(6,2),
        SALEDATE DATE
        );
    
    CREATETABLE PET (
        ID INTEGERNOTNULL,
        ANIMAL VARCHAR(20),
        QUANTITY INTEGER
        );
    
    ```
    
    ![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/1.1.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/1.1.png)
    
2. Now insert some records into the two newly created tables and show all the records of the two tables. Copy the code below and paste it to the textbox of the **Run SQL** page. Click **Run all**.
    
    ```sql
    
    INSERT INTO PETSALE VALUES
        (1,'Cat',450.09,100.47,'2018-05-29'),
        (2,'Dog',666.66,150.76,'2018-06-01'),
        (3,'Parrot',50.00,8.9,'2018-06-04'),
        (4,'Hamster',60.60,12,'2018-06-11'),
        (5,'Goldfish',48.48,3.5,'2018-06-14');
    
    INSERT INTO PET VALUES
        (1,'Cat',3),
        (2,'Dog',4),
        (3,'Hamster',2);
    
    SELECT * FROM PETSALE;
    SELECT * FROM PET;
    
    ```
    
    ![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/1.2.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/1.2.png)
    

# **Exercise 2: ALTER**

In this exercise, you will use the ALTER statement to add, delete, or modify columns in two of the existing tables created in exercise 1.

## **Task A: ALTER using ADD COLUMN**

1. Add a new **QUANTITY** column to the **PETSALE** table and show the altered table. Copy the code below and paste it to the textbox of the **Run SQL** page. Click **Run all**.
    
    ```sql
    
    ALTERTABLE PETSALE
    ADDCOLUMN QUANTITY INTEGER;
    
    SELECT *FROM PETSALE;
    
    ```
    
    ![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/2.A.1.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/2.A.1.png)
    
2. Now update the newly added **QUANTITY** column of the **PETSALE** table with some values and show all the records of the table. Copy the code below and paste it to the textbox of the **Run SQL** page. Click **Run all**.
    
    ```sql
    
    UPDATE PETSALESET QUANTITY = 9WHEREID = 1;
    UPDATE PETSALESET QUANTITY = 3WHEREID = 2;
    UPDATE PETSALESET QUANTITY = 2WHEREID = 3;
    UPDATE PETSALESET QUANTITY = 6WHEREID = 4;
    UPDATE PETSALESET QUANTITY = 24WHEREID = 5;
    
    SELECT *FROM PETSALE;
    
    ```
    
    ![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/2.A.2.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/2.A.2.png)
    

## **Task B: ALTER using DROP COLUMN**

1. Delete the **PROFIT** column from the **PETSALE** table and show the altered table. Copy the code below and paste it to the textbox of the **Run SQL** page. Click **Run all**.
    
    ```sql
    
    ALTERTABLE PETSALE
    DROPCOLUMN PROFIT;
    
    SELECT *FROM PETSALE;
    
    ```
    
    ![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/2.B.1.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/2.B.1.png)
    

## **Task C: ALTER using ALTER COLUMN**

1. Change the data type to **VARCHAR(20)** type of the column **PET** of the table **PETSALE** and show the altered table. Copy the code below and paste it to the textbox of the **Run SQL** page. Click **Run all**.
    
    ```sql
    
    ALTERTABLE PETSALE
    ALTERCOLUMN PETSETDATATYPE VARCHAR(20);
    
    SELECT *FROM PETSALE;
    
    ```
    
    ![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/2.C.1.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/2.C.1.png)
    
2. Now verify if the data type of the column **PET** of the table **PETSALE** changed to **VARCHAR(20)** type or not. Click on the 3 bar menu icon in the top left corner and click **Explore** > **Tables**. Find the **PETSALE** table from Schemas by clicking **Select All**. Click on the **PETSALE** table to open the Table Definition page of the table. Here, you can see all the current data type of the columns of the **PETSALE** table.
    
    ![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/2.C.2.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/2.C.2.png)
    

## **Task D: ALTER using RENAME COLUMN**

1. Rename the column **PET** to **ANIMAL** of the **PETSALE** table and show the altered table. Copy the code below and paste it to the textbox of the **Run SQL** page. Click **Run all**.
    
    ```sql
    
    ALTERTABLE PETSALE
    RENAMECOLUMN PETTO ANIMAL;
    
    SELECT *FROM PETSALE;
    
    ```
    
    ![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/2.D.1.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/2.D.1.png)
    

# **Exercise 3: TRUNCATE**

In this exercise, you will use the TRUNCATE statement to remove all rows from an existing table created in exercise 1 without deleting the table itself.

1. Remove all rows from the **PET** table and show the empty table. Copy the code below and paste it to the textbox of the **Run SQL** page. Click **Run all**.
    
    ```sql
    
    TRUNCATETABLE PETIMMEDIATE;
    
    SELECT *FROM PET;
    
    ```
    
    ![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/3.1.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/3.1.png)
    

# **Exercise 4: DROP**

In this exercise, you will use the DROP statement to delete an existing table created in exercise 1.

1. Delete the **PET** table and verify if the table still exists or not (SELECT statement won't work if a table doesn't exist). Copy the code below and paste it to the textbox of the **Run SQL** page. Click **Run all**.
    
    ```sql
    
    DROPTABLE PET;
    
    SELECT *FROM PET;
    
    ```
    
    ![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/4.1.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Labs_Coursera_V5/labs/Lab%20-%20CREATE%20-%20ALTER%20-%20TRUNCATE%20-%20DROP/images/4.1.png)
    

### **Congratulations! You have completed this Lab. You are ready for the next topic.**

### 

## **Author(s)**

- [Sandip Saha Joy](https://www.linkedin.com/in/sandipsahajoy/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork22-2022-01-01)

## **Changelog**

| Date | Version | Changed by | Change Description |
| --- | --- | --- | --- |
| 2020-12-24 | 1.1 | Steve Ryan | ID reviewed |
| 2020-12-07 | 1.0 | Sandip Saha Joy | Initial version created |

## 

### **© IBM Corporation 2020. All rights reserved.**