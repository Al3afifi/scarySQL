# commands

This is for my own reference to have quick back access to commands and their uses

'mysql' in bash to start up a connection \
make sure to end every line in mysql with ';'

*show databases;* will only list the database names.\
*create database **db_name**;* will create a database using that name.

Make sure to select the database by inputing `use db_name;`\

`show tables;` will list all the tables' names that are in this database;
`create table table_name` will create a new table, however don't end it there.

When creating a table, before the ';', list each column name and its variable type as such:\
`create table table_name (id int, name varchar(255), alive boolean);`

`describe table_name;` will display the vartypes and more info on each row of a table.

`insert into table_name values (1, "name");` will insert the respective values upon a table at the bottom of available rows;

`select * from table_name;` will show the values in a table in a human readable fashion.\
Can change the `*` to specify rows.\
Can add to end of line command `where name = "name"` to filter out results.\
Add `or` to add more filters.

`delete from table_name`*`filter;`* to remove rows from a table.

`update` with filter can help change and alter rows without fully deleting one.\
ex: `update table_name set last_name = NULL where first_name = "groot";` will remove the last name for groot.

`select * from table_name order by age asc;` will list in order all rows by column age.

`alter table table_name add column_name vartype;` will add a column to an existing table, filling blank details with NULL.
