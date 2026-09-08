# página 205 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 201 
•
Controls: DBAs maintain information security by access controls, database auditing, intrusion
detection, and vulnerability assessment tools.
Concepts and activities involved in setting up data security are discussed in Chapter 7. 
2.2.3.3 Create Storage Containers 
All data must be stored on a physical drive and organized for ease of load, search, and retrieval. Storage 
containers themselves may contain storage objects, and each level must be maintained appropriate to the level 
of the object. For example, relational databases have schemas that contain tables, and non-relational databases 
have filesystems that contain files. 
2.2.3.4 Implement Physical Data Models 
DBAs are typically responsible for creating and managing the complete physical data storage environment 
based on the physical data model. The physical data model includes storage objects, indexing objects, and any 
encapsulated code objects required to enforce data quality rules, connect database objects, and achieve database 
performance. 
Depending on the organization, data modelers may provide the data model and the DBAs implement the 
physical layout of the data model in storage. In other organizations, DBAs may take a skeleton of a physical 
model and add all the database-specific implementation details, including indexes, constraints, partitions or 
clusters, capacity estimates, and storage allocation details. 
For third-party database structures provided as part of an application, most data modeling tools allow reverse 
engineering of Commercial Off the Shelf (COTS) or Enterprise Resource Planning (ERP) system databases, as 
long as the modeling tool can read the storage tool catalog. These can be used to develop a Physical Model. 
DBAs or data modelers will still need to review and potentially update the physical model for application-based 
constraints or relationships; not all constraints and relationships are installed in database catalogs, especially for 
older applications where database abstraction was desired. 
Well-maintained physical models are necessary when DBAs are providing Data-as-a-Service. 
2.2.3.5 Load Data 
When first built, databases are empty. DBAs fill them. If the data to be loaded has been exported using a 
database utility, it may not be necessary to use a data integration tool to load it into the new database. Most 
database systems have bulk load capabilities, requiring that the data be in a format that matches the target 
database object, or having a simple mapping function to link data in the source to the target object.  
 

