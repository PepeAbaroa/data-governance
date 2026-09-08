# página 200 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

196 • DMBOK2 
production and production environments. They will need to create and document processes and procedures for 
administering the product with the least amount of effort and expense. 
2.2 Manage Databases 
Database support, as provided by DBAs and Network Storage Administrators (NSAs), is at the heart of data 
management. Databases reside on managed storage areas. Managed storage can be as small as a disk drive on a 
personal computer (managed by the OS), or as large as RAID arrays on a storage area network or SAN. Backup 
media is also managed storage.  
DBAs manage various data storage applications by assigning storage structures, maintaining physical databases 
(including physical data models and physical layouts of the data, such as assignments to specific files or disk 
areas), and establishing DBMS environments on servers.  
2.2.1 Understand Requirements 
2.2.1.1 Define Storage Requirements 
DBAs establish storage systems for DBMS applications and file storage systems to support NoSQL. NSAs and 
DBAs together play a vital role in establishing file storage systems. Data enters the storage media during normal 
business operations and, depending on the requirements, can stay permanently or temporarily. It is important to 
plan for adding additional space well in advance of when that space is actually needed. Doing any sort of 
maintenance in an emergency is a risk. 
All projects should have an initial capacity estimate for the first year of operations, and a growth projection for 
the following few years. Capacity and growth should be estimated not only for the space the data itself holds, 
but also for indexes, logs, and any redundant images such as mirrors. 
Data storage requirements must account for regulation related to data retention. For legal reasons, organizations 
are required to retain some data for set periods (see Chapter 9). In some cases, they may also be required to 
purge data after a defined period. It’s a good idea to discuss data retention needs with the data owners at design 
time and reach agreement on how to treat data through its lifecycle.  
The DBAs will work with application developers and other operations staff, including server and storage 
administrators, to implement the approved data retention plan. 
2.2.1.2 Identify Usage Patterns 
Databases have predictable usage patterns. Basic types of patterns include: 
 

