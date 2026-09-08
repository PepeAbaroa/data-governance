# página 136 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

132 • DMBOK2 
This first example (Figure 32) is a hierarchy and the second (Figure 33) is a network. In the first example, the 
Biology Workshop requires first taking the Biology Lecture and the Chemistry Lecture. Once the Biology 
Lecture is chosen as the prerequisite for the Biology Workshop, the Biology Lecture cannot be the prerequisite 
for any other courses. The second example allows the Biology Lecture to be the prerequisite for other courses as 
well. 
1.3.3.2.4.2 Binary Relationship 
An arity of two is also known as binary. A binary relationship, the most common on a traditional data model 
diagram, involves two entities. Figure 34, a UML class diagram, shows that both Student and Course are 
entities participating in a binary relationship. 
Figure 34 Binary Relationship 
1.3.3.2.4.3 Ternary Relationship 
An arity of three, known as ternary, is a relationship that includes three entities. An example in fact-based 
modeling (object-role notation) appears in Figure 35. Here Student can register for a particular Course in a 
given Semester.  
Figure 35 Ternary Relationship 
1.3.3.2.5 Foreign Key 
A foreign key is used in physical and sometimes logical relational data modeling schemes to represent a 
relationship. A foreign key may be created implicitly when a relationship is defined between two entities, 
depending on the database technology or data modeling tool, and whether the two entities involved have mutual 
dependencies. 
In the example shown in Figure 36, Registration contains two foreign keys, Student Number from Student and 
Course Code from Course. Foreign keys appear in the entity on the many side of the relationship, often called 
the child entity. Student and Course are parent entities and Registration is the child entity. 
Student
Course
-Attend
*
-Be attended by
*
Semester
Course
Student
 

