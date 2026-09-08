# página 145 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 141 
The class has Operations or Methods (also called its “behavior”). Class behavior is only loosely connected to 
business logic because it still needs to be sequenced and timed. In ER terms, the table has stored 
procedures/triggers.  
Class Operations can be: 
•
Public: Externally visible
•
Internally Visible: Visible to children Objects
•
Private: Hidden
In comparison, ER Physical models only offer Public access; all data is equally exposed to processes, queries, 
or manipulations. 
1.3.4.4 Fact-Based Modeling (FBM) 
Fact-Based Modeling, a family of conceptual modeling languages, originated in the late 1970s. These languages 
are based in the analysis of natural verbalization (plausible sentences) that might occur in the business domain. 
Fact-based languages view the world in terms of objects, the facts that relate or characterize those objects, and 
each role that each object plays in each fact. An extensive and powerful constraint system relies on fluent 
automatic verbalization and automatic checking against the concrete examples. Fact-based models do not use 
attributes, reducing the need for intuitive or expert judgment by expressing the exact relationships between 
objects (both entities and values). The most widely used of the FBM variants is Object Role Modeling (ORM), 
which was formalized as a first-order logic by Terry Halpin in 1989.  
1.3.4.4.1 Object Role Modeling (ORM or ORM2) 
Object‐Role Modeling (ORM) is a model‐driven engineering approach that starts with typical examples of 
required information or queries presented in any external formulation familiar to users, and then verbalizes 
these examples at the conceptual level, in terms of simple facts expressed in a controlled natural language. This 
language is a restricted version of natural language that is unambiguous, so the semantics are readily grasped by 
humans; it is also formal, so it can be used to automatically map the structures to lower levels for 
implementation (Halpin, 2015). 
Figure 42 illustrates an ORM model. 
Figure 42 ORM Model 
Semester
Course
Student
… in … enrolled in …
 

