Reference - https://www.stat.berkeley.edu/~spector/sql.pdf
https://www.studytonight.com/dbms/introduction-to-sql.php
https://stackoverflow.com/questions/9853586/how-can-i-join-multiple-sql-tables-using-the-ids

Introduction to SQL. Structure Query Language(SQL) is a database query language used for storing and managing data 
in Relational DBMS. ... Today almost all RDBMS(MySql, Oracle, Infomix, Sybase, MS Access) use SQL as the standard database 
query language. SQL is used to perform all types of data operations in RDBMS.

Since a single server can support many databases, each
containing many tables, with each table having a variety
of columns, it’s easy to get lost when you’re working with
databases. These commands will help figure out what’s
available:
I SHOW DATABASES;
I SHOW TABLES IN database;
I SHOW COLUMNS IN table;
I DESCRIBE table; - shows the columns and their
types
Joining 3 or more tables
SELECT TableA.*, TableB.*, TableC.*, TableD.*
FROM TableA
    JOIN TableB
        ON TableB.aID = TableA.aID
    JOIN TableC
        ON TableC.cID = TableB.cID
    JOIN TableD
        ON TableD.dID = TableA.dID
WHERE DATE(TableC.date)=date(now()) 
