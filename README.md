## Postgresql-Queries
### Database Queries 
##### Create Database
```sql
CREATE DATABASE database_name; 
```
##### Update Database Name
```sql
ALTER DATABSE "Current_database_name" RENAME TO "new_name"; 
```
##### Delete Database
```sql
DROP DATABASE Databasename; 
```
### Table Queries
##### Create Table
```sql
CREATE TABLE tablename (ID INT NOT NULL PRIMARY KEY , NAME VARCHAR(30));
```
##### Rename Table Name
```sql
ALTER TABLE tablename RENAME TO "new_table_name"; 
```
##### Add Column in Table
```sql
ALTER TABLE tablename add "column_name" VARCHAR(50); 
```
##### Update Coloumn name in table
```sql
ALTER TABLE tablename RENAME COLUMN "current_column_name" to "new_column_name"; 
```
##### Delete Column in Table
```sql
ALTER TABLE tablename DROP "column_name";
```
##### Change Data type of Column
```sql
ALTER TABLE tablename ALTER COLUMN id type int;
ALTER TABLE employee ALTER COLUMN "ColumnName" type varchar(100);
```
##### Remove Primary key from column 
```sql
ALTER TABLE tablename DROP CONSTRAINT tablename_pkey;
```
##### Add Primary Key in Column
```sql
ALTER TABLE tablename ADD PRIMARY KEY (column_name);
```
### Data In Table
##### Add Data in Table
```sql
INSERT INTO tablename VALUES(101, 'Akash Patel');
```
##### Update data in Table
```sql
UPDATE tablename SET name = 'Akash' WHERE id = 101;
```
##### Delete Whole Raw In Table
```sql
DELETE FROM employee WHERE id = 101;
```
### Create Foreign Key
###### In this query take project(project_id) from another table
```sql
create table ProjectCompany(company_name varchar(50), done_project_id integer references project(project_id));
```
### ENUMERATION Data Type
##### Create ENUM data type
```sql
CREATE TYPE mood as ENUM('sad','ok','happy');
CREATE TABLE person(name text, current_mood mood);
```
```mathematica
 employee_id | employee_name | department_id | department_id | department_name
-------------+---------------+---------------+---------------+-----------------
           1 | John          |             1 |             1 | HR
           2 | Jane          |             2 |             2 | IT
           3 | Alice         |             1 |             1 | HR
           4 | Bob           |             \N|             \N| \N
```


