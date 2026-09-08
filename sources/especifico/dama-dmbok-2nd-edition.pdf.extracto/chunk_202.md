# página 203 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 199 
Data in file system databases may be easier to restore than those in relational database management systems, 
which may have catalog information that needs to be updated during the data recovery, especially if the 
recovery is from logs instead of a full backup. 
It is critical to periodically test recovery of data. Doing so will reduce bad surprises during a disaster or 
emergency. Practice runs can be executed on non-production system copies with identical infrastructure and 
configuration, or if the system has a failover, on the secondary system. 
2.2.3 Develop Database Instances  
DBAs are responsible for the creation of database instances. Related activities include: 
•
Installing and updating DBMS software: DBAs install new versions of the DBMS software and
apply maintenance patches supplied by the DBMS vendor in all environments (from development to
production) as indicated by the vendor and vetted by and prioritized by DBA specialists, security
specialists, and management. This is a critical activity to ensure against vulnerability to attacks, as well
as to ensure ongoing data integrity in centralized and decentralized installations.
•
Maintaining multiple environment installations, including different DBMS versions: DBAs may
install and maintain multiple instances of DBMS software in sandbox, development, testing, user
acceptance testing, system acceptance testing, quality assurance, pre-production, hot-fix, disaster
recovery environments, and production, and manage migration of the DBMS software versions
through environments relative to applications and systems versioning and changes.
•
Installing and administering related data technology: DBAs may be involved in installing data
integration software and third party data administration tools.
2.2.3.1 Manage the Physical Storage Environment 
Storage environment management needs to follow traditional Software Configuration Management (SCM) 
processes or Information Technology Infrastructure Library (ITIL) methods to record modification to the 
database configuration, structures, constraints, permissions, thresholds, etc. DBAs need to update the physical 
data model to reflect the changes to the storage objects as part of a standard configuration management process. 
With agile development and extreme programming methods, updates to the physical data model play important 
roles in preventing design or development errors.  
DBAs need to apply the SCM process to trace changes and to verify that the databases in the development, test, 
and production environments have all of the enhancements included in each release – even if the changes are 
cosmetic or only in a virtualized data layer.  
The four procedures required to ensure a sound SCM process are configuration identification, configuration 
change control, configuration status accounting, and configuration audits. 
 

