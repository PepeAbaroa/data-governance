# página 135 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 131 
These cardinality symbols are illustrated in the following information engineering example of Student and 
Course.  
Figure 31 Cardinality Symbols 
The business rules are: 
•
Each Student may attend one or many Courses.
•
Each Course may be attended by one or many Students.
1.3.3.2.4 Arity of Relationships 
The number of entities in a relationship is the ‘arity’ of the relationship. The most common are unary, binary, 
and ternary relationships. 
1.3.3.2.4.1 Unary (Recursive) Relationship 
A unary (also known as a recursive or self-referencing) relationship involves only one entity. A one-to-many 
recursive relationship describes a hierarchy, whereas a many-to-many relationship describes a network or graph. 
In a hierarchy, an entity instance has at most one parent (or higher-level entity). In relational modeling, child 
entities are on the many side of the relationship, with parent entities on the one side of the relationship. In a 
network, an entity instance can have more than one parent.  
For example, a Course can require prerequisites. If, in order to take the Biology Workshop, one would first need 
to complete the Biology Lecture, the Biology Lecture is the prerequisite for the Biology Workshop. In the 
following relational data models, which use information engineering notation, one can model this recursive 
relationship as either a hierarchy or network: 
Figure 32 Unary Relationship - Hierarchy 
Figure 33 Unary Relationship - Network 
Course
Student
Attend
Course
Require as a pre-requisite
Course
Require as a pre-requisite
 

