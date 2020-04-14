# Database Normalization 
 **Database normalization** is a process used to organize a database into tables and columns.  The main idea with this is that a table should be about a specific topic and only supporting topics included.

 By limiting a table to one purpose you reduce the number of duplicate data contained within your database. This eliminates some issues stemming from database modifications.

 ## What is a Database Table?
A relational database is made up of several components, of which the table is most significant.  The database table is where all the data in a database is stored, and without tables, there would not be much use for relational databases.

 ## Reasons for Database Normalization
- The first is to minimize duplicate data
- the second is to minimize or avoid data modification issues
- the third is to simplify queries. 
These situations are modification anomalies. Database normalization fixes them. There are three modification anomalies that can occur:
1- Insert Anomaly
2- Update Anomaly
3- Search and Sort Issues


**Duplicated information presents two problems:**
- It increases storage and decrease performance.
- It becomes more difficult to maintain data changes.