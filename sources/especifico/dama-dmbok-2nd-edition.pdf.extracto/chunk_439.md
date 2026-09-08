# página 440 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

436 • DMBOK2 
•
Structure: How Metadata will be modeled for storage
•
Integration: The degree of integration of Metadata from different sources; rules for integration
•
Maintenance: Processes and rules for updating Metadata (logging and referring for approval)
•
Management: Roles and responsibilities for managing Metadata
•
Quality: Metadata quality requirements
•
Security: Some Metadata cannot be exposed because it will reveal the existence of highly protected
data
2.3 Define Metadata Architecture 
A Metadata Management system must be capable of extracting Metadata from many sources. Design the 
architecture to be capable of scanning the various Metadata sources and periodically updating the repository. 
The system must support the manual updates of Metadata, requests, searches, and lookups of Metadata by 
various user groups. 
A managed Metadata environment should isolate the end user from the various and disparate Metadata sources. 
The architecture should provide a single access point for the Metadata repository. The access point must supply 
all related Metadata resources transparently to the user. Users should be able to access Metadata without being 
aware of the differing environments of the data sources. In analytics and Big Data solutions, the interface may 
have largely user-defined functions (UDF) to draw on various data sets, and the Metadata exposure to the end 
user is inherent to those customizations. With less reliance on UDF in solutions, end users will be gathering, 
inspecting, and using data sets more directly and various supporting Metadata is usually more exposed.  
Design of the architecture depends on the specific requirements of the organization. Three technical 
architectural approaches to building a common Metadata repository mimic the approaches to designing data 
warehouses: centralized, distributed, and hybrid (see Section 1.3.6). These approaches all take into account 
implementation of the repository, and how the update mechanisms operate.  
2.3.1 Create MetaModel 
Create a data model for the Metadata repository, or metamodel, as one of the first design steps after the 
Metadata strategy is complete and the business requirements are understood. Different levels of metamodel may 
be developed as needed; a high-level conceptual model, that explains the relationships between systems, and a 
lower level metamodel that details the attributions, to describe the elements and processes of a model. In 
addition to being a planning tool and a means of articulating requirements, the metamodel is in itself a valuable 
source of Metadata.  
 

