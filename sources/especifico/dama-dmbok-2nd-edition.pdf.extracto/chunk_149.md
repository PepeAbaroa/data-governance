# página 150 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

146 • DMBOK2 
Figure 47 Dimensional Conceptual Model 
1.3.5.2 Logical 
A logical data model is a detailed representation of data requirements, usually in support of a specific usage 
context, such as application requirements. Logical data models are still independent of any technology or 
specific implementation constraints. A logical data model often begins as an extension of a conceptual data 
model.  
In a relational logical data model, the conceptual data model is extended by adding attributes. Attributes are 
assigned to entities by applying the technique of normalization (see Section 1.3.6), as shown in Figure 48. There 
is a very strong relationship between each attribute and the primary key of the entity in which it resides. For 
instance, School Name has a strong relationship to School Code. For example, each value of a School Code 
brings back at most one value of a School Name. 
Figure 48 Relational Logical Data Model 
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
Student
Student Number
School Code (FK)
Student First Name
Student Last Name
Student Birth Date
Application
Application Number
Student Number (FK)
Application Submission Date
School
School Code
School Name
Submit
Contain
 

