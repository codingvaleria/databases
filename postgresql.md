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
)

## Drop Tables
DROP TABLE table_name

## View Tables
\d - view all tables
\d table_name - view particular table

# View Contents of a table
- SELECT * FROM table_name
- SELECT column_name FROM table_name


# Postgress Datatypes 
[Postgress datatypes](https://www.postgresql.org/docs/current/datatype.html)

## Insert into tables
INSERT INTO table_name (
    column1,
    column2,
    column3,
) 
VALUES('column1', column2, 'column3'....)

