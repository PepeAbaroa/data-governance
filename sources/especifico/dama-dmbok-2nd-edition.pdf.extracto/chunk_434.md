# página 435 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

METADATA MANAGEMENT • 431 
1.3.6 Types of Metadata Architecture 
Like other forms of data, Metadata has a lifecycle. Conceptually, all Metadata management solutions include 
architectural layers that correspond to points in the Metadata lifecycle:  
•
Metadata creation and sourcing
•
Metadata storage in one or more repositories
•
Metadata integration
•
Metadata delivery
•
Metadata usage
•
Metadata control and management
Different architectural approaches can be used to source, store, integrate, maintain, and make Metadata 
accessible to consumers.  
1.3.6.1 Centralized Metadata Architecture 
A centralized architecture consists of a single Metadata repository that contains copies of Metadata from the 
various sources. Organizations with limited IT resources, or those seeking to automate as much as possible, may 
choose to avoid this architecture option. Organizations seeking a high degree of consistency within the common 
Metadata repository can benefit from a centralized architecture. 
Advantages of a centralized repository include: 
•
High availability, since it is independent of the source systems
•
Quick Metadata retrieval, since the repository and the query reside together
•
Resolved database structures not affected by the proprietary nature of third party or commercial
systems
•
Extracted Metadata may be transformed, customized, or enhanced with additional Metadata that may
not reside in the source system, improving quality
Some limitations of the centralized approach include: 
•
Complex processes are necessary to ensure that changes in source Metadata are quickly replicated into
the repository
•
Maintenance of a centralized repository can be costly
•
Extraction could require custom modules or middleware
•
Validation and maintenance of customized code can increase the demands on both internal IT staff and
the software vendors
Figure 85 shows how Metadata is collected in a standalone Metadata repository with its own internal Metadata 
store. The internal store is populated through a scheduled import (arrows) of the Metadata from the various 
tools. In turn, the centralized repository exposes a portal for the end users to submit their queries. The Metadata 
portal passes the request to the centralized Metadata repository. The centralized repository will fulfill the 
 

