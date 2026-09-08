# página 189 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 185 
parent/child relationships: each parent can have many children, but each child has only one parent (also known 
as a 1-to-many relationship). Directory trees are an example of a hierarchy. XML also uses a hierarchical 
model. It can be represented as a relational database, although the actual structure is that of a tree traversal path. 
1.3.8.2 Relational 
People sometimes think that relational databases are named for the relation between tables. This is not the case. 
Relational databases are based on set theory and relational algebra, where data elements or attributes (columns) 
are related into tuples (rows). (See Chapter 5.) Tables are sets of relations with identical structure. Set 
operations (like union, intersect, and minus) are used to organize and retrieve data from relational databases, in 
the form of Structured Query Language (SQL). In order to write data, the structure (schema) has to be known in 
advance (schema on write). Relational databases are row-oriented. 
The database management system (DBMS) of a relational database is called RDBMS. A relational database is 
the predominant choice in storing data that constantly changes. Variations on relational databases include 
Multidimensional and Temporal.  
1.3.8.2.1 Multidimensional 
Multidimensional database technologies store data in a structure that allows searching using several data 
element filters simultaneously. This type of structure is used most frequently in Data Warehousing and Business 
Intelligence. Some of these database types are proprietary, although most large databases have cube technology 
built in as objects. Access to the data uses a variant of SQL called MDX or Multidimensional eXpression. 
1.3.8.2.2 Temporal 
A temporal database is a relational database with built-in support for handling data involving time. The 
temporal aspects usually include valid time and transaction time. These attributes can be combined to form bi-
temporal data.  
•
Valid time is the timeframe when a fact is true with respect to the entity it represents in the real world.
•
Transaction time is the period during which a fact stored in the database is considered true.
It is possible to have timelines other than Valid Time and Transaction Time, such as Decision Time, in the 
database. In that case, the database is called a multi-temporal database as opposed to a bi-temporal database. 
Temporal databases enable application developers and DBAs to manage current, proposed, and historical 
versions of data in the same database.  
 

