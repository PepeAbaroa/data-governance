# página 181 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 177 
Loosely coupled systems require component databases to construct their own federated schema. A user will 
typically access other component database systems by using a multi-database language, but this removes any 
levels of location transparency, forcing the user to have direct knowledge of the federated schema. A user 
imports the data required from other component databases, and integrates it with their own to form a federated 
schema.  
Tightly coupled systems consist of component systems that use independent processes to construct and publish 
an integrated federated schema, as illustrated in Figure 57. The same schema can apply to all parts of the 
federation, with no data replication. 
Figure 57 Coupling 
1.3.4.2.2 Blockchain Database 
Blockchain databases are a type of federated database used to securely manage financial transactions. They can 
also be used for contract management or exchange of health information. There are two types of structures: 
individual records and blocks. Each transaction has a record. The database creates chains of time-bound groups 
of transactions (blocks) that also contain information from the previous block in the chain. Hash algorithms are 
used to create information about transactions to store in blocks while the block is the end of the chain. Once a 
new block is created, the old block hash should never change, which means that no transactions contained 
within that block may change. Any change to transactions or blocks (tampering) will be apparent when the hash 
values no longer match. 
1.3.4.3 Virtualization / Cloud Platforms 
Virtualization (also called ‘cloud computing’) provides computation, software, data access, and storage services 
that do not require end-user knowledge of the physical location and configuration of the system that delivers the 
F
F
F
Tightly Coupled
Loosely Coupled
User View
User View
Location A
Location A
Location B
Location B
map
map
map
map
 

[5 imágenes en esta página]
