# página 142 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

138 • DMBOK2 
1.3.4.2 Dimensional 
The concept of dimensional modeling started from a joint research project conducted by General Mills and 
Dartmouth College in the 1960’s.33 In dimensional models, data is structured to optimize the query and analysis 
of large amounts of data. In contrast, operational systems that support transaction processing are optimized for 
fast processing of individual transactions. 
Dimensional data models capture business questions focused on a particular business process. The process 
being measured on the dimensional model in Figure 40 is Admissions. Admissions can be viewed by the Zone 
the student is from, School Name, Semester, and whether the student is receiving financial aid. Navigation can 
be made from Zone up to Region and Country, from Semester up to Year, and from School Name up to School 
Level. 
Figure 40 Axis Notation for Dimensional Models 
The diagramming notation used to build this model – the ‘axis notation’ – can be a very effective 
communication tool with those who prefer not to read traditional data modeling syntax. 
Both the relational and dimensional conceptual data models can be based on the same business process (as in 
this example with Admissions). The difference is in the meaning of the relationships, where on the relational 
model the relationship lines capture business rules, and on the dimensional model, they capture the navigation 
paths needed to answer business questions. 
33 http://bit.ly/2tsSP7w. 
Admissions
Zone
Country
Region
Financial Aid
Semester
Year
Yes/No
School
Geography
Calendar
Name
Level
 

