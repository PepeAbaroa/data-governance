# página 436 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

432 • DMBOK2 
request from the collected Metadata. In this type of implementation, the capability to pass the request from the 
user to various tools directly is not supported. Global search across the Metadata collected from the various tool 
is possible due to the collection of various Metadata in the centralized repository. 
Figure 85 Centralized Metadata Architecture 
1.3.6.2 Distributed Metadata Architecture 
A completely distributed architecture maintains a single access point. The Metadata retrieval engine responds to 
user requests by retrieving data from source systems in real time; there is no persistent repository. In this 
architecture, the Metadata management environment maintains the necessary source system catalogs and lookup 
information needed to process user queries and searches effectively. A common object request broker or similar 
middleware protocol accesses these source systems. 
Advantages of distributed Metadata architecture include: 
•
Metadata is always as current and valid as possible because it is retrieved from its source
•
Queries are distributed, possibly improving response and process time
•
Metadata requests from proprietary systems are limited to query processing rather than requiring a
detailed understanding of proprietary data structures, therefore minimizing the implementation and
maintenance effort required
•
Development of automated Metadata query processing is likely simpler, requiring minimal manual
intervention
•
Batch processing is reduced, with no Metadata replication or synchronization processes
Distributed architectures also have limitations: 
•
No ability to support user-defined or manually inserted Metadata entries since there is no repository in
which to place these additions
•
Standardization of presenting Metadata from various systems
•
Query capabilities are directly affected by the availability of the participating source systems
•
The quality of Metadata depends solely on the participating source systems
Metadata Portal
ENTERPRISE METADATA REPOSITORY
BI Tools
Modeling 
Tools
ETL Tools
Services 
Repository
DBMS 
Tools
Reference 
Data
Data 
Quality 
Tools
Messaging 
Tools
Configura-
tion Tools
 

[3 imágenes en esta página]
