# página 156 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

152 • DMBOK2 
The subtyping relationship implies that all of the properties from the supertype are inherited by the subtype. In 
the relational example shown in Figure 52, University and High School are subtypes of School. 
Figure 52 Supertype and Subtype Relationships 
Subtyping reduces redundancy on a data model. It also makes it easier to communicate similarities across what 
otherwise would appear to be distinct and separate entities. 
2. Activities
This section will briefly cover the steps for building conceptual, logical, and physical data models, as well as 
maintaining and reviewing data models. Both forward engineering and reverse engineering will be discussed. 
2.1 Plan for Data Modeling 
A plan for data modeling contains tasks such as evaluating organizational requirements, creating standards, and 
determining data model storage. 
The deliverables of the data modeling process include: 
•
Diagram: A data model contains one or more diagrams. The diagram is the visual that captures the
requirements in a precise form. It depicts a level of detail (e.g., conceptual, logical, or physical), a
scheme (relational, dimensional, object-oriented, fact-based, time-based, or NoSQL), and a notation
within that scheme (e.g., information engineering, unified modeling language, object-role modeling).
•
Definitions: Definitions for entities, attributes, and relationships are essential to maintaining the
precision on a data model.
•
Issues and outstanding questions: Frequently the data modeling process raises issues and questions
that may not be addressed during the data modeling phase. In addition, often the people or groups
responsible for resolving these issues or answering these questions reside outside of the group building
the data model. Therefore, often a document is delivered that contains the current set of issues and
outstanding questions. An example of an outstanding issue for the student model might be, “If a
School
University
High School
Student
Application
Contain
Submit
 

