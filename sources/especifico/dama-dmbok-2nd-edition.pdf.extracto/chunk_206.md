# página 207 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 203 
•
Working with system programmers and network administrators to tune operating systems, networks,
and transaction processing middleware to work with the database.
•
Dedicating appropriate storage and enabling the database to work with storage devices and storage
management software. Storage management software optimizes the use of different storage
technologies for cost-effective storage of older, less-frequently referenced data, by migrating that data
to less expensive storage devices. This results in more rapid retrieval time for core data. DBAs work
with storage administrators to set up and monitor effective storage management procedures.
•
Providing volumetric growth studies to support storage acquisition and general data lifecycle
management activities of retention, tuning, archiving, backup, purging, and disaster recovery.
•
Working with system administrators to provide operating workloads and benchmarks of deployed data
assets that support SLA management, charge-back calculations, server capacity, and lifecycle rotation
within the prescribed planning horizon.
2.2.4.1 Set Database Performance Service Levels 
System performance, data availability and recovery expectations, and expectations for teams to respond to 
issues are usually governed through Service Level Agreements (SLAs) between IT data management services 
organizations and data owners (Figure 61). 
Figure 61 SLAs for System and Database Performance 
Typically, an SLA will identify the timeframes during which the database is expected to be available for use. 
Often an SLA will identify a specified maximum allowable execution time for a few application transactions (a 
mix of complex queries and updates). If the database is not available as agreed to, or if process execution times 
violate the SLA, the data owners will ask the DBA to identify and remediate the causes of the problem. 
Service Level 
Agreement
System Performance
System Availability
System Recovery
Service Level 
Agreement
Database Performance
Database Availability
Data Owners
Data 
Stewards
IT Data 
Management 
Services
DBA
NSA
 

[9 imágenes en esta página]
