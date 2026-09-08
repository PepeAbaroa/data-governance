# página 177 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 173 
Data lifecycle management includes implementing policies and procedures for acquisition, migration, retention, 
expiration, and disposition of data. It is prudent to prepare checklists to ensure all tasks are performed at a high 
level of quality. DBAs should use a controlled, documented, and auditable process for moving application 
database changes to the Quality Assurance or Certification (QA) and Production environments. A manager-
approved service request or change request usually initiates the process. The DBA should have a back out plan 
to reverse changes in case of problems. 
1.3.3 Administrators 
The role of Database Administrator (DBA) is the most established and the most widely adopted data 
professional role. DBAs play the dominant roles in Data Storage and Operations, and critical roles in Data 
Security (see Chapter 7), the physical side of data modeling, and database design (see Chapter 5). DBAs 
provide support for development, test, QA, and special use database environments. 
DBAs do not exclusively perform all the activities of Data Storage and Operations. Data stewards, data 
architects, network administrators, data analysts, and security analysts participate in planning for performance, 
retention, and recovery. These teams may also participate in obtaining and processing data from external 
sources. 
Many DBAs specialize as Production, Application, Procedural and Development DBAs. Some organizations 
also have Network Storage Administrators (NSA) who specialize in supporting the data storage system 
separately from the data storage applications or structures.  
In some organizations, each specialized role reports to a different organization within IT. Production DBAs may 
be part of production infrastructure or application operations support groups. Application, Development, and 
Procedural DBAs are sometimes integrated into application development organizations. NSAs usually are 
connected to Infrastructure organizations. 
1.3.3.1 Production DBA 
Production DBAs take primary responsibility for data operations management, including: 
•
Ensuring the performance and reliability of the database, through performance tuning, monitoring,
error reporting, and other activities
•
Implementing backup and recovery mechanisms to ensure data can be recovered if lost in any
circumstance
•
Implementing mechanisms for clustering and failover of the database, if continual data availability data
is a requirement
•
Executing other database maintenance activities, such as implementing mechanisms for archiving data
 

