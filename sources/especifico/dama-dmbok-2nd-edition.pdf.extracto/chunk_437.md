# página 438 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

434 • DMBOK2 
Various challenges are apparent in this approach. The design forces the Metadata repository to contain the latest 
version of the Metadata source and forces it to manage changes to the source, as well. Changes must be trapped 
systematically, and then resolved. Additional sets of process interfaces to tie the repository back to the Metadata 
source(s) must be built and maintained. 
Figure 87 Hybrid Metadata Architecture 
Figure 87 illustrates how common Metadata from different sources is collected in a centralized Metadata store. 
Users submit their queries to the Metadata portal, which passes the request to a centralized repository. The 
centralized repository will try to fulfill the user request from the common Metadata collected initially from the 
various sources. As the request becomes more specific or the user needs more detailed Metadata then the 
centralized repository will delegate down to the specific source to research the specific details. Global search 
across the various tools is available due to the common Metadata collected in the centralized repository. 
2. Activities
2.1 Define Metadata Strategy 
A Metadata strategy describes how an organization intends to manage its Metadata and how it will move from 
current state to future state practices. A Metadata strategy should provide a framework for development teams 
to improve Metadata management. Developing Metadata requirements will help clarify the drivers of the 
strategy and identify potential obstacles to enacting it.  
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
BI 
Metadata
Modeling 
Metadata
ETL 
Metadata
Services 
Metadata
DBMS 
Metadata
Reference
Metadata
Data 
Quality 
Metadata
Messaging 
Metadata
Configura-
tion 
Metadata
 

[5 imágenes en esta página]
