# página 178 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

174 • DMBOK2 
As part of managing data operations, Production DBAs create the following deliverables: 
•
A production database environment, including an instance of the DBMS (Database Management
System) on the supporting server, of a sufficient size and capacity to ensure adequate performance,
configured for the appropriate level of security, reliability, and availability. Database System
Administration is responsible for the DBMS environment.
•
Mechanisms and processes for controlled implementation of changes to databases in the production
environment
•
Mechanisms for ensuring the availability, integrity, and recoverability of data in response to all
circumstances that could result in loss or corruption of data
•
Mechanisms for detecting and reporting any error that occurs in the database, the DBMS, or the data
server
•
Database availability, recovery, and performance in accordance with service level agreements
•
Mechanisms and processes for monitoring database performance as workloads and data volumes vary
1.3.3.2 Application DBA 
An application DBA is responsible for one or more databases in all environments (development / test, QA, and 
production), as opposed to database systems administration for any of these environments. Sometimes, 
application DBAs report to the organizational units responsible for development and maintenance of the 
applications supported by their databases. There are pros and cons to staffing application DBAs.  
Application DBAs are viewed as integral members of an application support team. By focusing on a specific 
database, they can provide better service to application developers. However, application DBAs can easily 
become isolated and lose sight of the organization’s overall data needs and common DBA practices. 
Application DBAs collaborate closely with data analysts, modelers, and architects.  
1.3.3.3 Procedural and Development DBAs 
Procedural DBAs lead the review and administration of procedural database objects. A procedural DBA 
specializes in development and support of procedural logic controlled and execute by the DBMS: stored 
procedures, triggers, and user-defined functions (UDFs). The procedural DBA ensures this procedural logic is 
planned, implemented, tested, and shared (reused).  
Development DBAs focus on data design activities including creating and managing special use databases, such 
as ‘sandbox’ or exploration areas.  
In many cases, these two functions are combined under one position. 
 

