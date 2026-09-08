# página 190 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

186 • DMBOK2 
1.3.8.3 Non-relational 
Non-relational databases can store data as simple strings or complete files. Data in these files can be read in 
different ways, depending on the need (this characteristic is referred to as ‘schema on read’). Non-relational 
databases may be row-oriented, but this is not required. 
A non-relational database provides a mechanism for storage and retrieval of data that employs less constrained 
consistency models than traditional relational databases. Motivations for this approach include simplicity of 
design, horizontal scaling, and finer control over availability.  
Non-relational databases are usually referred to as NoSQL (which stands for “Not Only SQL”). The primary 
differentiating factor is the storage structure itself, where the data structure is no longer bound to a tabular 
relational design. It could be a tree, a graph, a network, or a key-value pairing. The NoSQL tag emphasizes that 
some editions may in fact support conventional SQL directives. These databases are often highly optimized data 
stores intended for simple retrieval and appending operations. The goal is improved performance, especially 
with respect to latency and throughput. NoSQL databases are used increasingly in Big Data and real-time web 
applications. (See Chapter 5.) 
1.3.8.3.1 Column-oriented 
Column-oriented databases are used mostly in Business Intelligence applications because they can compress 
redundant data. For example, a state ID column only has unique values, instead of one value for each of a 
million rows. 
There are trade-offs between column-oriented (non-relational) and row-oriented (usually relational) 
organization.  
•
Column-oriented organization is more efficient when an aggregate needs to be computed over many
rows. This only holds true for a notably smaller subset of all columns of data, because reading that
smaller subset of data can be faster than reading all data.
•
Column-oriented organization is more efficient when new values of a column are supplied for all rows
at once, because that column data can be written efficiently to replace old column data without
touching any other columns for the rows.
•
Row-oriented organization is more efficient when many columns of a single row are required at the
same time, and when row-size is relatively small, as the entire row can be retrieved with a single disk
seek.
•
Row-oriented organization is more efficient when writing a new row if all of the row data is supplied
at the same time; the entire row can be written with a single disk seek.
•
In practice, row-oriented storage layouts are well suited for Online Transaction Processing (OLTP)-
like workloads, which are more heavily loaded with interactive transactions. Column-oriented storage
 

