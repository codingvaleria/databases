# Database
- is a place where we can 
    - store
    - manipulate
    - retrieve data.

# PostgreSQL
- postgress is the database engine
- sql is the language that allows us to have commands

# Sql
- Manage data held in relational databases 

- data is stored in tables made of rows and columns
- attributes make the column values make rows

# Relational database 
- is a relation between one or more tables.

# Manipulating DBs
1. using GUI Client - basically an application 
2. Terminal/CMD
3. Application- using a serverside app

# Database Commands

## CREATE Database
- To create a new database
    CREATE DATABASE nameofdatabase;

## Connect to Database


## Switch to different database
 \c database_name

## Delete Database  
DROP DATABASE database_name;    

## Create Tables
CREATE TABLE table_name(
    Column name + data type + constraints if any
);

## Drop Tables
DROP TABLE table_name;

## View Tables
\d - view all tables
\d table_name - view particular table

# View Contents of a table
- SELECT * FROM table_name;
- SELECT column_name FROM table_name;


# Postgress Datatypes 
[Postgress datatypes](https://www.postgresql.org/docs/current/datatype.html)

## Insert into tables
INSERT INTO table_name (
    column1,
    column2,
    column3,
) 
VALUES('column1', 'column2', 'column3'....);

# Sort Data
SELECT * FROM table_name ORDER BY column_name ASC;

to combine multiple columns
SELECT * FROM table_name ORDER BY column_nam1, column _name2 DESC;

# Distinct
- used to find unique details(non-duplicates) from a db.

SELECT DISTINCT column_name FROM table_name ORDER BY column_name;

# Where Clause and AND and OR
- Where allows to filter data based on condition
SELECT * FROM table_name WHERE column_name = 'some text';

- And - to add conditions
SELECT * FROM table_name WHERE column_name = 'some text' AND column_name = 'some text';

SELECT * FROM table_name WHERE column_name = 'some text' AND (column_name = 'some text' OR column_name = 'some text');

# Comparison Operators
- <, >, = <=, =>  <>(not equal)

## Arithmetic

# LIMIT, Offset & Fetch
- Limit ; to limit a certain conditon

##### Limit
SELECT * FROM table_name LIMIT no;

#### Offset 
 Dictates the number of rows to skip from the beginning of the returned data before presenting the results.

SELECT * FROM table_name OFFSET 15 LIMIT 10;

#### Fetch 
- Used as an alternative to limit
SELECT * FROM table_name OFFSET 5 FETCH FIRST 5 ROW ONLY;

# IN
Returns a query matching an array of keywords given.

SELECT * FROM table_name WHERE country_of_birth IN ('China', 'Brazil', 'France');

# Between
- To select data within a range.

## Like and ilike
- Used to match text values against a pattern using wild cards
SELECT * FROM person WHERE email LIKE '%@google.com';

- ilike is case insensitive

# GROUP BY
- allows to group based on a column and gives their quantity
