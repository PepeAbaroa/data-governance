# página 148 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

144 • DMBOK2 
1.3.4.6.1 Document 
Instead of taking a business subject and breaking it up into multiple relational structures, document databases 
frequently store the business subject in one structure called a document. For example, instead of storing 
Student, Course, and Registration information in three distinct relational structures, properties from all three 
will exist in a single document called Registration.  
1.3.4.6.2 Key-value 
Key-value databases allow an application to store its data in only two columns (‘key’ and ‘value’), with the 
feature of storing both simple (e.g., dates, numbers, codes) and complex information (unformatted text, video, 
music, documents, photos) stored within the ‘value’ column.  
1.3.4.6.3 Column-oriented 
Out of the four types of NoSQL databases, column-oriented is closest to the RDBMS. Both have a similar way 
of looking at data as rows and values. The difference, though, is that RDBMSs work with a predefined structure 
and simple data types, such as amounts and dates, whereas column-oriented databases, such as Cassandra, can 
work with more complex data types including unformatted text and imagery. In addition, column-oriented 
databases store each column in its own structure. 
1.3.4.6.4 Graph 
A graph database is designed for data whose relations are well represented as a set of nodes with an 
undetermined number of connections between these nodes. Examples where a graph database can work best are 
social relations (where nodes are people), public transport links (where nodes could be bus or train stations), or 
roadmaps (where nodes could be street intersections or highway exits). Often requirements lead to traversing 
the graph to find the shortest routes, nearest neighbors, etc., all of which can be complex and time-consuming to 
navigate with a traditional RDMBS. Graph databases include Neo4J, Allegro, and Virtuoso. 
1.3.5 Data Model Levels of Detail 
In 1975, the American National Standards Institute’s Standards Planning and Requirements Committee 
(SPARC) published their three-schema approach to database management. The three key components were: 
•
Conceptual: This embodies the ‘real world’ view of the enterprise being modeled in the database. It
represents the current ‘best model’ or ‘way of doing business’ for the enterprise.
 

