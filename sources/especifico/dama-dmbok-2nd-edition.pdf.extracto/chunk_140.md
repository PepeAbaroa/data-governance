# página 141 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 137 
Table 10 Scheme to Database Cross Reference 
Scheme 
Relational Database 
Management System 
(RDBMS) 
Multidimensional 
Database Management 
System (MDBMS) 
Object Databases 
Document 
Column 
Graph 
Key-Value 
Relational 
CDM 
LDM 
PDM 
CDM 
LDM 
CDM 
LDM 
CDM 
LDM 
CDM 
LDM 
CDM 
LDM 
CDM 
LDM 
Dimensional 
CDM 
LDM 
PDM 
CDM 
LDM 
PDM 
Object-Oriented 
CDM 
LDM 
PDM 
CDM 
LDM 
PDM 
Fact-Based 
CDM 
LDM 
PDM 
CDM 
LDM 
CDM 
LDM 
CDM 
LDM 
CDM 
LDM 
CDM 
LDM 
CDM 
LDM 
Time-Based 
PDM 
NoSQL 
PDM 
PDM 
PDM 
PDM 
PDM 
1.3.4.1 Relational 
First articulated by Dr. Edward Codd in 1970, relational theory provides a systematic way to organize data so 
that they reflected their meaning (Codd, 1970). This approach had the additional effect of reducing redundancy 
in data storage. Codd’s insight was that data could most effectively be managed in terms of two-dimensional 
relations. The term relation was derived from the mathematics (set theory) upon which his approach was based. 
(See Chapter 6.) 
The design objectives for the relational model are to have an exact expression of business data and to have one 
fact in one place (the removal of redundancy). Relational modeling is ideal for the design of operational 
systems, which require entering information quickly and having it stored accurately (Hay, 2011).  
There are several different kinds of notation to express the association between entities in relational modeling, 
including Information Engineering (IE), Integration Definition for Information Modeling (IDEF1X), Barker 
Notation, and Chen Notation. The most common form is IE syntax, with its familiar tridents or ‘crow’s feet’ to 
depict cardinality. (See Figure 39.) 
Figure 39 IE Notation 
Course
Student
Attend
 

