# página 210 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

206 • DMBOK2 
each process locking resources needed by the other. Most DBMSs will automatically terminate one of 
these processes after an interval of time. These types of problems are often the result of poor coding, 
either in the database or in the application. 
•
Inaccurate database statistics: Most relational DBMSs have a built-in query optimizer, which relies
on stored statistics about the data and indexes to make decisions about how to execute a given query
most effectively. These statistics should be updated frequently, especially in active databases. Failure
to do so will result in poorly performing queries.
•
Poor coding: Perhaps the most common cause of poor database performance is poorly coded SQL.
Query coders need a basic understanding of how the SQL query optimizer works. They should code
SQL in a way that takes maximum advantage of the optimizer’s capabilities. Some systems allow
encapsulation of complex SQL in stored procedures, which can be pre-compiled and pre-optimized,
rather than embedded in application code or in script files.
•
Inefficient complex table joins: Use views to pre-define complex table joins. In addition, avoid using
complex SQL (e.g., table joins) in database functions; unlike stored procedures, these are opaque to the
query optimizer.
•
Insufficient indexing: Code complex queries and queries involving large tables to use indexes built on
the tables. Create the indexes necessary to support these queries. Be careful about creating too many
indexes on heavily updated tables, as this will slow down update processing.
•
Application activity: Ideally, applications should be running on a server separate from the DBMS, so
that they are not competing for resources. Configure and tune database servers for maximum
performance. In addition, the new DBMSs allow application objects, such as Java and .NET classes, to
be encapsulated in database objects and executed in the DBMS. Be careful about making use of this
capability. It can be very useful in certain cases, but executing application code on the database server
may affect the interoperability, application architecture, and performance of database processes.
•
Overloaded servers: For DBMSs that support multiple databases and applications, there may be a
breaking point where the addition of more databases has an adverse effect on the performance of
existing databases. In this case, create a new database server. In addition, relocate databases that have
grown very large, or that are being used more heavily than before, to a different server. In some cases,
address problems with large databases by archiving less-used data to another location, or by deleting
expired or obsolete data.
•
Database volatility: In some cases, large numbers of table inserts and deletes over a short while can
create inaccurate database distribution statistics. In these cases, turn off updating database statistics for
these tables, as the incorrect statistics will adversely affect the query optimizer.
•
Runaway queries: Users may unintentionally submit queries that use a majority of the system’s
shared resources. Use rankings or query governors to kill or pause these queries until they can be
evaluated and improved.
 

