# página 437 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

METADATA MANAGEMENT • 433 
Figure 86 Distributed Metadata Architecture 
Figure 86 illustrates a distributed Metadata architecture. There is no centralized Metadata repository store and 
the portal passes the users’ requests to the appropriate tool to execute. As there is no centralized store for the 
Metadata to be collected from the various tools, every request has to be delegated down to the sources; hence, 
no capability exist for a global search across the various Metadata sources. 
1.3.6.3 Hybrid Metadata Architecture 
A hybrid architecture combines characteristics of centralized and distributed architectures. Metadata still moves 
directly from the source systems into a centralized repository. However, the repository design only accounts for 
the user-added Metadata, the critical standardized items, and the additions from manual sources. 
The architecture benefits from the near-real-time retrieval of Metadata from its source and enhanced Metadata 
to meet user needs most effectively, when needed. The hybrid approach lowers the effort for manual IT 
intervention and custom-coded access functionality to proprietary systems. The Metadata is as current and valid 
as possible at the time of use, based on user priorities and requirements. Hybrid architecture does not improve 
system availability. 
The availability of the source systems is a limitation, because the distributed nature of the back-end systems 
handles processing of queries. Additional overhead is required to link those initial results with the Metadata 
augmentation in the central repository before presenting the result set to the end user. 
Many organizations can benefit from a hybrid architecture, including those that have rapidly-changing 
operational Metadata, those that need consistent, uniform Metadata, and those that experience substantial 
growth in Metadata and Metadata sources. Organizations with more static Metadata and smaller Metadata 
growth profiles may not see the maximum potential from this architecture alternative. 
1.3.6.4 Bi-Directional Metadata Architecture 
Another advanced architectural approach is bi-directional Metadata architecture, which allows Metadata to 
change in any part of the architecture (source, data integration, user interface) and then feedback is coordinated 
from the repository (broker) into its original source.  
Metadata Portal
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
 

[2 imágenes en esta página]
