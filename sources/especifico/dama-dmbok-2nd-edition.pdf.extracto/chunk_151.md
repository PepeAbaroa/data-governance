# página 152 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

148 • DMBOK2 
1.3.5.3 Physical 
A physical data model (PDM) represents a detailed technical solution, often using the logical data model as a 
starting point and then adapted to work within a set of hardware, software, and network tools. Physical data 
models are built for a particular technology. Relational DBMSs, for example, should be designed with the 
specific capabilities of a database management system in mind (e.g., IBM DB2, UDB, Oracle, Teradata, 
Sybase, Microsoft SQL Server, or Microsoft Access).  
Figure 50 illustrates a relational physical data model. In this data model, School has been denormalized into the 
Student entity to accommodate a particular technology. Perhaps whenever a Student is accessed, their school 
information is as well and therefore storing school information with Student is a more performant structure 
than having two separate structures. 
Figure 50 Relational Physical Data Model 
Because the physical data model accommodates technology limitations, structures are often combined 
(denormalized) to improve retrieval performance, as shown in this example with Student and School. 
Figure 51 illustrates a dimensional physical data model (usually a star schema, meaning there is one structure 
for each dimension). 
Similar to the relational physical data model, this structure has been modified from its logical counterpart to 
work with a particular technology to ensure business questions can be answered with simplicity and speed. 
1.3.5.3.1 Canonical 
A variant of a physical scheme is a Canonical Model, used for data in motion between systems. This model 
describes the structure of data being passed between systems as packets or messages. When sending data 
through web services, an Enterprise Service Bus (ESB), or through Enterprise Application Integration (EAI), 
the canonical model describes what data structure the sending service and any receiving services should use. 
These structures should be designed to be as generic as possible to enable re-use and simplify interface 
requirements.  
This structure may only be instantiated as a buffer or queue structure on an intermediary messaging system 
(middleware) to hold message contents temporarily.  
STUDENT
STUDENT_NUM
STUDENT_FIRST_NAM
STUDENT_LAST_NAM
STUDENT_BIRTH_DT
SCHOOL_CD
SCHOOL_NAM
APPLICATION
APPLICATION_NUM
STUDENT_NUM (FK)
APPLICATION_SUBMISSION_DT
Submit
 

