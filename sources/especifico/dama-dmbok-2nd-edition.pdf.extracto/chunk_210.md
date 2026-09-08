# página 211 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 207 
After the cause of the problem is identified, the DBA will take whatever action is needed to resolve the 
problem, including working with application developers to improve and optimize the database code, and 
archiving or deleting data that is no longer actively needed by application processes. In exceptional cases for 
OLTP-type databases, the DBA may consider working with the data modeler restructure the affected portion of 
the database. Do this only after other measures (e.g., the creation of views and indexes and the rewriting of SQL 
code) have been tried, and only after careful consideration of the possible consequences, such as loss of data 
integrity or the increase in complexity of SQL queries against denormalized tables.  
For read-only reporting and analytical databases, denormalization for performance and ease of access is the rule 
rather than the exception, and poses no threat or risk. 
2.2.4.5 Maintain Alternate Environments 
Databases do not appear once and remain unchanged. Business rules change, business processes change, and 
technology changes. Development and test environments enable changes to be tested before they are brought 
into a production environment. DBAs can make whole or subset copies of database structures and data onto 
other environments to enable development and testing of system changes. There are several types of alternate 
environments.  
•
Development environments are used to create and test changes that will be implemented in
production. Development must be maintained to closely resemble the production environment, though
with scaled down resources.
•
Test environments serve several purposes: QA, integration testing, UAT, and performance testing.
The test environment ideally also has the same software and hardware as production. In particular,
environments used for performance testing should not be scaled down in resources.
•
Sandboxes or experimental environments are used to test hypotheses and develop new uses of data.
The DBAs generally set up, grant access to, and monitor usage of these environments. They should
also ensure that sandboxes are isolated and do not adversely affecting production operations.
•
Alternate production environments are required to support offline backups, failover, and resiliency
support systems. These systems should be identical to the production systems, although the backup
(and recovery) system can be scaled down in compute capacity, since it is mostly dedicated to I/O
activities.
2.2.5 Manage Test Data Sets 
Software testing is labor-intensive and accounts for nearly half of the cost of the system development. Efficient 
testing requires high quality test data, and this data must be managed. Test data generation is a critical step in 
software testing. 
 

