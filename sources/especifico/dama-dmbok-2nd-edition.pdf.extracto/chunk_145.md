# página 146 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

142 • DMBOK2 
1.3.4.4.2 Fully Communication Oriented Modeling (FCO-IM) 
FCO-IM is similar in notation and approach to ORM. The numbers in Figure 43 are references to verbalizations 
of facts. For example, 2 might refer to several verbalizations including “Student 1234 has first name Bill.” 
Figure 43 FCO-IM Model 
1.3.4.5 Time-Based 
Time-based patterns are used when data values must be associated in chronological order and with specific time 
values. 
1.3.4.5.1 Data Vault 
The Data Vault is a detail-oriented, time-based, and uniquely linked set of normalized tables that support one or 
more functional areas of business. It is a hybrid approach, encompassing the best of breed between third normal 
form (3NF, to be discussed in Section 1.3.6) and star schema. Data Vaults are designed specifically to meet the 
needs of enterprise data warehouses. There are three types of entities: hubs, links, and satellites. The Data Vault 
design is focused around the functional areas of business with the hub representing the primary key. The links 
provide transaction integration between the hubs. The satellites provide the context of the hub primary key 
(Linstedt, 2012).  
In Figure 44, Student and Course are hubs, which represent the main concepts within a subject. Attendance is a 
link, which relates two hubs to each other. Student Contact, Student Characteristics, and Course 
Description are satellites that provide the descriptive information on the hub concepts and can support varying 
types of history. 
Anchor Modeling is a technique suited for information that changes over time in both structure and content. It 
provides graphical notation used for conceptual modeling similar to traditional data modeling, with extensions 
for working with temporal data. Anchor Modeling has four basic modeling concepts: anchors, attributes, ties, 
2
Student
3
Course
1
Semester
4
5
6
Attendance
 

