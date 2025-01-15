## **SQL Cheat Sheet: Basics - SELECT, INSERT, UPDATE, DELETE, COUNT, DISTINCT, LIMIT**

![https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Module%202/images/IDSNlogo.png](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/Module%202/images/IDSNlogo.png)

| Command | Syntax | Description | Example |
| --- | --- | --- | --- |
| SELECT | SELECT column1, column2, ... FROM table_name; | SELECT statement is used to fetch data from a database. | SELECT city FROM placeofinterest; |
| WHERE | SELECT column1, column2, ...FROM table_name WHERE condition; | WHERE clause is used to extract only those records that fulfill a specified condition. | SELECT * FROM placeofinterest WHERE city == 'Rome' ; |
| COUNT | SELECT COUNT * FROM table_name ; | COUNT is a function that takes the name of a column as argument and counts the number of rows when the column is not NULL. | SELECT COUNT(country) FROM placeofinterest WHERE country='Canada'; |
| DISTINCT | SELECT DISTINCT columnname FROM table_name; | DISTINCT function is used to specify that the statement is a query which returns unique values in specified columns. | SELECT DISTINCT country FROM placeofinterest WHERE type='historical'; |
| LIMIT | SELECT * FROM table_name LIMIT number; | LIMIT is a clause to specify the maximum number of rows the result set must have. | SELECT * FROM placeofinterest WHERE airport="pearson" LIMIT 5; |
| INSERT | INSERT INTO table_name (column1,column2,column3...) VALUES(value1,value2,value3...); | INSERT is used to insert new rows in the table. | INSERT INTO placeofinterest (name,type,city,country,airport) VALUES('Niagara Waterfalls','Nature','Toronto','Canada','Pearson'); |
| UPDATE | UPDATE table_name SET[[column1]=[VALUES]] WHERE [condition]; | UPDATE used to update the rows in the table. | UPDATE placeofinterest SET name = 'Niagara Falls' WHERE name = "Niagara Waterfalls"; |
| DELETE | DELETE FROM table_name WHERE [condition]; | DELETE statement is used to remove rows from the table which are specified in the WHERE condition. | DELETE FROM placeofinterest WHERE city IN ('Rome','Vienna'); |

## **Author(s)**

[Malika Singla](https://www.linkedin.com/in/malika-goyal-04798622/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork20127838-2022-01-01)

## **Changelog**

| Date | Version | Changed by | Change Description |
| --- | --- | --- | --- |
| 2021-07-27 | 1.0 | Malika | Initial Version |