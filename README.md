# Database-Project-
Project Requirements
Design a good relational database schema: Use the ideas of the relational data model to
design a good database schema according to the above requirements. Make sure to
indicate primary and foreign keys. Pease note that the next paragraph already gives
further information about the part of the database pertaining to parts, suppliers and
orders. Some hints: It is a good idea to first design an EER diagram according to the
above requirements. Then map your EER diagram to a relational database schema. You
might need to modify a couple of schemas to make sure that all schemas are in 3NF.
1. Create some tables and fill with data from json files: The process of implementing the
entire database schema could be tedious once the design has been completed. You are
required to create (in MySQL) only tables pertaining to parts, suppliers and orders as
follows.
The file parts_100.json contains 100 json parts. The file parts_table.sql contains the
definition of the MySQL table parts. The bash script j2sql_parts.sh contains commands
that read the 100 json parts and insert corresponding tuples into the MySQL table parts.
Your first task here is to simply change the username/password/database names in
j2sql_parts.sh and execute that script in your account so that it creates and fills with data
the parts MySQL table in your account. The file suppliers_100.json contains a json array
of 100 suppliers. The file orders_4000.json contains 4000 json orders. Your second task
here is to (a) create a file make_tables.sql containing definitions of the rest of the
MySQL tables pertaining to suppliers and orders; (b) create and execute a bash script file
j2sql_supp+order.sh containing commands that read the 100 json suppliers and the 4000
json orders, and insert corresponding tuples into the MySQL tables defined in your
make_tables.sql. Make sure that your j2sql_supp+order.sh begins by assigning your own
username/password/database values to variables and uses these variables in subsequent
commands, as opposed to your actual username/password/database values. Note that
your script might rely on some other script(s) and that you are required to submit all
files/scripts/programs pertaining to this task.
All the above will be tested on the Linux server dbcourse.cs.smu.ca.
2. Write and present a web application that allows the user to perform the following
operations:
  o Show table: the user enters the name of a table, and the application prints the
  contents of the table.
  o Add new supplier: the user enters the attribute values pertaining to a supplier and
  the application inserts the corresponding rows in the database. The program
  should consider the case where the new supplier cannot be inserted.
  o Annual Expenses for Parts: the user enters a start year and an end year, and the
  application shows the total amount of money paid for parts in each of the selected
  years.
  o Budget Projection: the user enters a number N of years and an inflation rate value
  (e.g, 2%), and the application shows the total amount of money that would be
  spent in each of the next N years by applying inflation (starting after the most
  recent full year, 2022).


Here is a quick link to the app
http://dbcourse.cs.smu.ca/~u10/project/public_html/index.php
  
