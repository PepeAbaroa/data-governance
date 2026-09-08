# página 157 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 153 
Student leaves and then returns, are they assigned a different Student Number or do they keep their 
original Student Number?” 
•
Lineage: For physical and sometimes logical data models, it is important to know the data lineage, that
is, where the data comes from. Often lineage takes the form of a source/target mapping, where one can
capture the source system attributes and how they populate the target system attributes. Lineage can
also trace the data modeling components from conceptual to logical to physical within the same
modeling effort. There are two reasons why lineage is important to capture during the data modeling.
First, the data modeler will obtain a very strong understanding of the data requirements and therefore is
in the best position to determine the source attributes. Second, determining the source attributes can be
an effective tool to validate the accuracy of the model and the mapping (i.e., a reality check).
2.2 Build the Data Model 
To build the models, modelers often rely heavily on previous analysis and modeling work. They may study 
existing data models and databases, refer to published standards, and incorporate any data requirements. After 
studying these inputs, they start building the model. Modeling is a very iterative process (Figure 53). Modelers 
draft the model, and then return to business professionals and business analysts to clarify terms and business 
rules. They then update the model and ask more questions (Hoberman, 2014).  
Figure 53 Modeling is Iterative 
2.2.1 Forward Engineering 
Forward engineering is the process of building a new application beginning with the requirements. The CDM is 
completed first to understand the scope of the initiative and the key terminology within that scope. Then the 
LDM is completed to document the business solution, followed by the PDM to document the technical solution. 
2.2.1.1 Conceptual Data Modeling 
Creating the CDM involves the following steps: 
Elicit
Document
Increase precision
Ask more questions
 

[6 imágenes en esta página]
