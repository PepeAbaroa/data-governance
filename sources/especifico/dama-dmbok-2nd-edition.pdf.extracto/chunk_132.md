# página 133 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 129 
in object-oriented schemes the terms class or object are often used, in time-based schemes the terms hub, 
satellite, and link are often used, and in NoSQL schemes terms such as document or node are used.  
Entity aliases can also vary based on level of detail. (The three levels of detail will be discussed in Section 
1.3.5.) An entity at the conceptual level can be called a concept or term, an entity at the logical level is called an 
entity (or a different term depending on the scheme), and at the physical level the terms vary based on database 
technology, the most common term being table. 
1.3.3.1.2 Graphic Representation of Entities 
In data models, entities are generally depicted as rectangles (or rectangles with rounded edges) with their names 
inside, such as in Figure 29, where there are three entities: Student, Course, and Instructor. 
Figure 29 Entities 
1.3.3.1.3 Definition of Entities 
Entity definitions are essential contributors to the business value of any data model. They are core Metadata. 
High quality definitions clarify the meaning of business vocabulary and provide rigor to the business rules 
governing entity relationships. They assist business and IT professionals in making intelligent business and 
application design decisions. High quality data definitions exhibit three essential characteristics:  
•
Clarity: The definition should be easy to read and grasp. Simple, well-written sentences without
obscure acronyms or unexplained ambiguous terms such as sometimes or normally.
•
Accuracy: The definition is a precise and correct description of the entity. Definitions should be
reviewed by experts in the relevant business areas to ensure that they are accurate.
•
Completeness: All of the parts of the definition are present. For example, in defining a code, examples
of the code values are included. In defining an identifier, the scope of uniqueness in included in the
definition.
1.3.3.2 Relationship 
A relationship is an association between entities (Chen, 1976). A relationship captures the high-level 
interactions between conceptual entities, the detailed interactions between logical entities, and the constraints 
between physical entities.  
Student
Course
Instructor
 

