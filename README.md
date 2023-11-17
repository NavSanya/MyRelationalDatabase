# MyRelationalDatabase

### Game Plan
##### IDEA:
###### SELECT:
* Get all = SELECT *
* Get  ___ = SELECT ___
###### FROM:
* From table ___ = FROM ___
###### WHERE:
* Where ___ = WHERE ___
* greater than = >
* less than = <
* at least = >=
* at most = <=
* equal to = ==
###### JOIN:
* combine tables __ on __ = JOIN ___ on ___
###### GROUP BY:
* find sum/avg/... of column ___ of table ___ =   SELECT column1, aggregate_function(column2) FROM table_name GROUP BY column1;
###### HAVING:
* where ___ = HAVING ____
###### ORDER BY:
* ___ in asc/desc order = ORDER BY ___ ASC/DESC
###### INSERT INTO:
* Add [values] to table ___ in columns [names] = INSERT INTO table_name (column1, column2, column3, ...) VALUES (value1, value2, value3, ...)
###### CREATE TABLE:
* create a table ___ with the following column and datatypes: [col1: datatype1, col2: datatype2 ...]
###### UPDATE:
* update ___ in table ___ with ___ = UPDATE table_name SET column1 = value1, column2 = value2, ... WHERE condition;

-----------------------------------------------------------------------------

### Game Plan
* Each Individual Table is converted to a CSV File
###  DB Details
##### * Columns in original db
* rank - int
* name - string
* year - int
* rating - float
* genre - string/list
* certificate - String(Can make an enumerator)
* run_time - hours and minutes
* tagline - String
* budget - int (Long)
* box_office - int
* casts - list string
* directors - list string
* writers - list strings

### Tables we make
#### * Movie Essentials
* rank(PK), name, year
#### * Movie Details for viewers
* rank(FK), rating, genre, tagline, certificate
#### * Movie details for media
* rank(FK), budget, box_office
#### * Movie Makers
* rank(FK), casts, directors, writers
