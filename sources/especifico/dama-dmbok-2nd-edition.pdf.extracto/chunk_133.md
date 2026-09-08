# página 134 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

130 • DMBOK2 
1.3.3.2.1 Relationship Aliases 
The generic term relationship can go by other names. Relationship aliases can vary based on scheme. In 
relational schemes the term relationship is often used, dimensional schemes the term navigation path is often 
used, and in NoSQL schemes terms such as edge or link are used, for example. Relationship aliases can also 
vary based on level of detail. A relationship at the conceptual and logical levels is called a relationship, but a 
relationship at the physical level may be called by other names, such as constraint or reference, depending on 
the database technology. 
1.3.3.2.2 Graphic Representation of Relationships 
Relationships are shown as lines on the data modeling diagram. See Figure 30 for an Information Engineering 
example. 
Figure 30 Relationships 
In this example, the relationship between Student and Course captures the rule that a Student may attend 
Courses. The relationship between Instructor and Course captures the rule than an Instructor may teach 
Courses. The symbols on the line (called cardinality) capture the rules in a precise syntax. (These will be 
explained in Section 1.3.3.2.3.) A relationship is represented through foreign keys in a relational database and 
through alternative methods for NoSQL databases such as through edges or links. 
1.3.3.2.3 Relationship Cardinality 
In a relationship between two entities, cardinality captures how many of one entity (entity instances) 
participates in the relationship with how many of the other entity. Cardinality is represented by the symbols that 
appear on both ends of a relationship line. Data rules are specified and enforced through cardinality. Without 
cardinality, the most one can say about a relationship is that two entities are connected in some way.  
For cardinality, the choices are simple: zero, one, or many. Each side of a relationship can have any 
combination of zero, one, or many (‘many’ means could be more than ‘one’). Specifying zero or one allows us 
to capture whether or not an entity instance is required in a relationship. Specifying one or many allows us to 
capture how many of a particular instance participates in a given relationship. 
Instructor
Student
Course
Teach
Attend
 

