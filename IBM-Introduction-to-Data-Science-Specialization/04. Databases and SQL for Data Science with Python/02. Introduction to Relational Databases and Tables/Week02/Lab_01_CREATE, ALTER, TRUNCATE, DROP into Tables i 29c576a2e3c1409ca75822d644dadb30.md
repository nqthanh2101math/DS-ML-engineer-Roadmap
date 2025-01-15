# Lab_01_CREATE, ALTER, TRUNCATE, DROP into Tables in MySQL using phpMyAdmin

![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/SN_web_lightmode.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/SN_web_lightmode.png)

# **Hands-on Lab: CREATE, ALTER, TRUNCATE, DROP into Tables in MySQL using phpMyAdmin**

**Estimated time needed:** 20 minutes

In this lab, you will learn how to create tables and load data in the MySQL database service using the phpMyAdmin graphical user interface (GUI) tool.

## **Software Used in this Lab**

In this lab, you will use [MySQL](https://www.mysql.com/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDB0110ENSkillsNetwork24601058-2021-01-01). MySQL is a Relational Database Management System (RDBMS) designed to efficiently store, manipulate, and retrieve data.

![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Create%20Tables%20and%20Load%20Data%20in%20MySQL%20using%20phpMyAdmin/images/mysql.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Create%20Tables%20and%20Load%20Data%20in%20MySQL%20using%20phpMyAdmin/images/mysql.png)

To complete this lab you will utilize MySQL relational database service available as part of IBM Skills Network Labs (SN Labs) Cloud IDE. SN Labs is a virtual lab environment used in this course.

## **Database Used in this Lab**

**Mysql_learners** database has been used in this lab.

## **Objectives**

After completing this lab, you will be able to use phpMyAdmin with MySQL to:

- Create a database.
- Create a new table in a database.
- Add, delete, or modify columns in an existing table.
- Remove all rows from an existing table without deleting the table itself.
- Delete an existing table in a database

## **Exercise**

In this exercise through different tasks, you will learn how to create tables and load data in the MySQL database service using the phpMyAdmin graphical user interface (GUI) tool.

### **Task A: Create a database**

1. Click on **Skills Network Toolbox**. In **Database** section, click **MySQL**.

To start the MySQL click **Start**.

![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/php1.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/php1.png)

1. Once **MySQL** has started, click on **phpMyAdmin button** to open **phpMyAdmin** in the same window.

![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/php2.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/php2.png)

1. You will see the phpMyAdmin GUI tool.

![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Create%20Tables%20and%20Load%20Data%20in%20MySQL%20using%20phpMyAdmin/images/2.4.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Create%20Tables%20and%20Load%20Data%20in%20MySQL%20using%20phpMyAdmin/images/2.4.png)

1. In the tree-view, click **New** to create a new empty database. Then enter **Mysql_Learners** as the name of the database and select **utf8_general_ci** and click **Create**.
    
    UTF-8 is the most commonly used character encoding for content or data.
    
    Proceed to Task B.
    
    ![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/images/db1.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/images/db1.png)
    

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
ALTER TABLE table_name
ADD COLUMN column_name data_type column_constraint;

ALTER TABLE table_nameDROP 
COLUMN column_name;

ALTER TABLE table_nameALTER 
COLUMN column_name SET DATA TYPE data_type;

ALTER TABLE table_name
CHANGE current_column_name new_column_name;
```

**How does the syntax of a TRUNCATE statement look?**

```sql
TRUNCATE TABLE table_name;
```

**How does the syntax of a DROP statement look?**

```sql
DROP TABLE table_name;
```

In this exercise, you will use the CREATE statement to create two new tables using Db2.

1. You need to create two tables, **PETSALE** and **PET**. To create the two tables PETSALE and PET, copy the code below and paste it to the textarea of the **SQL** page. Click **Go**.
    
    ```sql
    CREATE TABLE PETSALE (
    		ID INTEGER NOT NULL,
    		PET CHAR(20),    
    		SALEPRICE DECIMAL(6,2),    
    		PROFIT DECIMAL(6,2),    
    		SALEDATE DATE    
    		);
    
    CREATE TABLE PET (    
    		ID INTEGER NOT NULL,    
    		ANIMAL VARCHAR(20),    
    		QUANTITY INTEGER    
    		);
    ```
    

![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/createtable.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/createtable.png)

1. Now insert some records into the two newly created tables and show all the records of the two tables. Copy the code below and paste it to the textarea of the **SQL** page. Click **Go**.
    
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
    

![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/insert.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/insert.png)

In this exercise, you will use the ALTER statement to add, delete, or modify columns in two of the existing tables created in exercise 1.

## **Task A: ALTER using ADD COLUMN**

1. Add a new **QUANTITY** column to the **PETSALE** table and show the altered table. Copy the code below and paste it to the textarea of the **SQL** page. Click **Go**..
    
    ```sql
    ALTER TABLE PETSALE
    ADD COLUMN QUANTITY INTEGER;
    
    SELECT * FROM PETSALE;
    ```
    

![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/alter.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/alter.png)

1. Now update the newly added **QUANTITY** column of the **PETSALE** table with some values and show all the records of the table. Copy the code below and paste it to textarea of the **SQL** page. Click **Go**.
    
    ```sql
    UPDATE PETSALE SET QUANTITY = 9 WHERE ID = 1;
    UPDATE PETSALE SET QUANTITY = 3 WHERE ID = 2;
    UPDATE PETSALE SET QUANTITY = 2 WHERE ID = 3;
    UPDATE PETSALE SET QUANTITY = 6 WHERE ID = 4;
    UPDATE PETSALE SET QUANTITY = 24 WHERE ID = 5;
    
    SELECT * FROM PETSALE;
    ```
    

![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/update.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/update.png)

## **Task B: ALTER using DROP COLUMN**

1. Delete the **PROFIT** column from the **PETSALE** table and show the altered table. Copy the code below and paste it to the textarea of the **SQL** page. Click **Go**.
    
    ```sql
    ALTER TABLE PETSALE
    DROP COLUMN PROFIT;
    
    SELECT * FROM PETSALE;
    ```
    

![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/alter_drop.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/alter_drop.png)

## **Task C: ALTER using ALTER COLUMN**

1. Change the data type to **VARCHAR(20)** type of the column **PET** of the table **PETSALE** and show the altered table. Copy the code below and paste it to the textarea of the **SQL** page. Click **Go**.
    
    ```sql
    ALTER TABLE PETSALE CHANGE PET  PET VARCHAR(20);
    SELECT * FROM PETSALE;
    ```
    

![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/changedatatype.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/changedatatype.png)

## **Task D: ALTER using RENAME COLUMN**

1. Rename the column **PET** to **ANIMAL** of the **PETSALE** table and show the altered table. Copy the code below and paste it to the textarea of the **SQL** page. Click **Go**.
    
    ```sql
    ALTER TABLE `PETSALE` CHANGE `PET` `ANIMAL` varchar(20);
    
    SELECT * FROM PETSALE;
    ```
    
    ![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/renamecolumn.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/renamecolumn.png)
    

In this exercise, you will use the TRUNCATE statement to remove all rows from an existing table created in exercise 1 without deleting the table itself.

1. Remove all rows from the **PET** table and show the empty table. Copy the code below and paste it to the textarea of the **SQL** page. Click **Go**.
    
    ```sql
    TRUNCATE TABLE PET ;
    
    SELECT * FROM PET;
    ```
    

![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/truncate.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/truncate.png)

In this exercise, you will use the DROP statement to delete an existing table created in exercise 1.

1. Delete the **PET** table and verify if the table still exists or not (SELECT statement won’t work if a table doesn’t exist). Copy the code below and paste it to the textarea of the **SQL** page. Click **Go**.
    
    ```sql
    DROP TABLE PET;
    
    SELECT * FROM PET;
    ```
    

![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/drop.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/MySQL/week2/images/drop.png)

### **Congratulations! You have completed this lab, and you are ready for the next topic.**

[Lakshmi Holla](https://www.linkedin.com/in/lakshmi-holla-b39062149/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork22-2022-01-01)

[Malika Singla](https://www.linkedin.com/in/malika-goyal-04798622/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork22-2022-01-01)

## **Changelog**

| Date | Version | Changed by | Change Description |
| --- | --- | --- | --- |
| 2022-10-28 | 0.4 | Appalabhaktula Hema | Updated instructions |
| 2022-07-27 | 0.3 | Lakshmi Holla | updated html tag |
| 2022-06-04 | 0.2 | Lakshmi Holla, Malika Singla | Updated the MySQL starting commands |
| 2021-11-01 | 0.1 | Lakshmi Holla, Malika Singla | Initial Version |

### **© IBM Corporation 2021. All rights reserved.**

# Summary

1. Build a proper table
    
    ```sql
    CREATE TABLE PETSALE (
        ID INTEGER NOT NULL,
        PET CHAR(20),
        SALEPRICE DECIMAL(6,2),
        PROFIT DECIMAL(6,2),
        SALEDATE DATE
        );
        
    CREATE TABLE PET (
        ID INTEGER NOT NULL,
        ANIMAL VARCHAR(20),
        QUANTITY INTEGER
        );
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
    
2. Add a new **QUANTITY** column to the **PETSALE** table and show the altered table
    
    ```sql
    ALTER TABLE `PETSALE`
    ADD COLUMN `QUANTITY` integer;
    ```
    
3. update the newly added **QUANTITY** column of the **PETSALE** table with some values and show all the records of the table
    
    ```sql
    UPDATE `PETSALE` SET `QUANTITY` = 9 WHERE `ID` = 1; 
    UPDATE `PETSALE` SET `QUANTITY` = 8 WHERE `ID` = 2; 
    UPDATE `PETSALE` SET `QUANTITY` = 9 WHERE `ID` = 3; 
    UPDATE `PETSALE` SET `QUANTITY` = 7 WHERE `ID` = 4; 
    UPDATE `PETSALE` SET `QUANTITY` = 3 WHERE `ID` = 5; 
    ```
    
4. Delete the **PROFIT** column from the **PETSALE** table and show the altered table
    
    ```sql
    ALTER TABLE `PETSALE`
    DROP COLUMN `PROFIT`;
    ```
    
5. Change the data type to **VARCHAR(20)** type of the column **PET** of the table **PETSALE**
 and show the altered table
    
    ```sql
    ALTER TABLE `PETSALE` CHANGE `PET` `PET` VARCHAR(20)
    ```
    
6. Rename the column **PET** to **ANIMAL** of the **PETSALE** table and show the altered table
    
    ```sql
    ALTER TABLE `PETSALE` COLUMN `PET` `ANIMAL`  varchar(20);
    ```
    
7. use the `TRUNCATE` statement to remove **all rows** from an existing table
    
    ```sql
    TRUNCATE TABLE Name_table ;
    ```
    
8. Delete the **PET** table and verify if the table still exists or not (SELECT statement won’t work if a table doesn’t exist)
    
    ```sql
    DROP TABLE `PET`;
    SELECT * FROM `PET`;
    ```