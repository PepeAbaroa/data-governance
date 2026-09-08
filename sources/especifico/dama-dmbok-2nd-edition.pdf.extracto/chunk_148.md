# página 149 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 145 
•
External: The various users of the database management system operate on sub-sets of the total
enterprise model that are relevant to their particular needs. These subsets are represented as ‘external
schemas’.
•
Internal: The ‘machine view’ of the data is described by the internal schema. This schema describes
the stored representation of the enterprise’s information (Hay, 2011).
These three levels most commonly translate into the conceptual, logical, and physical levels of detail, 
respectively. Within projects, conceptual data modeling and logical data modeling are part of requirements 
planning and analysis activities, while physical data modeling is a design activity. This section provides an 
overview of conceptual, logical, and physical data modeling. In addition, each level will be illustrated with 
examples from two schemes: relational and dimensional. 
1.3.5.1 Conceptual 
A conceptual data model captures the high-level data requirements as a collection of related concepts. It 
contains only the basic and critical business entities within a given realm and function, with a description of 
each entity and the relationships between entities.  
For example, if we were to model the relationship between students and a school, as a relational conceptual data 
model using the IE notation, it might look like Figure 46. 
Figure 46 Relational Conceptual Model 
Each School may contain one or many Students, and each Student must come from one School. In addition, 
each Student may submit one or many Applications, and each Application must be submitted by one Student. 
The relationship lines capture business rules on a relational data model. For example, Bob the student can attend 
County High School or Queens College, but cannot attend both when applying to this particular university. In 
addition, an application must be submitted by a single student, not two and not zero. 
Recall Figure 40, which is reproduced below as Figure 47. This dimensional conceptual data model using the 
Axis notation, illustrates concepts related to school: 
School
Application
Student
Contain
Submit
 

