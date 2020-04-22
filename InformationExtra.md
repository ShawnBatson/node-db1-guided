# Relational Databases

-   A collection of rows === a table
-   Each one of those rows === a record

## Features

-   Give names and data types to columns
-   Each row has a unique identifier (primary key)
-   Columns can link to other colums in separate tables (foreign keys)

Data Definition Language (DQL)
SELECT <columns> FROM <table> WHERE <column> = <value>;

Data Manipulation Language (DML)

INSERT INTO <table> (<columns>) VALUES (<value>)
UPDATE <table> SET <Column> = <new value> WHERE <column> = <Value>
DELETE FROM <table> WHERE <column> = <value>

# Different levels of Database Abstractions in javascript

-   No abstraction, write SQL statements and send them directly to the database

-   ORM (Object Relational Mapper), High level of abstraction (Sequelize.org)

-   Query Builder, a library that allows us to write SQL with Javascript functions
    -   table.insert({}).into("table_name") instead of INSERT INTO "table_name" VALUES ();
