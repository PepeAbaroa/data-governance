# página 140 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

136 • DMBOK2 
•
Range: Domains that allow all values of the same data type that are between one or more minimum
and/or maximum values. Some ranges can be open-ended. For example, OrderDeliveryDate must be
between OrderDate and three months in the future.
•
Rule-based: Domains defined by the rules that values must comply with in order to be valid. These
include rules comparing values to calculated values or other attribute values in a relation or set. For
example, ItemPrice must be greater than ItemCost.
1.3.4 Data Modeling Schemes 
The six most common schemes used to represent data are: Relational, Dimensional, Object-Oriented, Fact-
Based, Time-Based, and NoSQL. Each scheme uses specific diagramming notations (see Table 9).  
Table 9 Modeling Schemes and Notations 
Scheme 
Sample Notations 
Relational 
Information Engineering (IE) 
Integration Definition for Information Modeling (IDEF1X) 
Barker Notation 
Chen 
Dimensional 
Dimensional 
Object-Oriented 
Unified Modeling Language (UML) 
Fact-Based 
Object Role Modeling (ORM or ORM2) 
Fully Communication Oriented Modeling (FCO-IM) 
Time-Based 
Data Vault 
Anchor Modeling 
NoSQL 
Document 
Column 
Graph 
Key-Value 
This section will briefly explain each of these schemes and notations. The use of schemes depends in part on the 
database being built, as some are suited to particular technologies, as shown in Table 10. 
For the relational scheme, all three levels of models can be built for RDBMS, but only conceptual and logical 
models can be built for the other types of databases. This is true for the fact-based scheme as well. For the 
dimensional scheme, all three levels of models can be built for both RDBMS and MDBMS databases. The 
object-oriented scheme works well for RDBMS and object databases.  
The time-based scheme is a physical data modeling technique primarily for data warehouses in a RDBMS 
environment. The NoSQL scheme is heavily dependent on the underlying database structure (document, 
column, graph, or key-value), and is therefore a physical data modeling technique. Table 10 illustrates several 
important points including that even with a non-traditional database such as one that is document-based, a 
relational CDM and LDM can be built followed by a document PDM. 
 

