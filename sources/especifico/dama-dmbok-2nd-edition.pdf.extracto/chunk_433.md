# página 434 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

430 • DMBOK2 
1.3.5.12 Modeling Tools and Repositories 
Data modeling tools are used to build various types of data models: conceptual, logical, and physical. These 
tools produce Metadata relevant to the design of the application or system model, like subject areas, logical 
entities, logical attributes, entity and attribute relationships, super types and subtypes, tables, columns, indexes, 
primary and foreign keys, integrity constraints, and other types of attribution from the models. Metadata 
repositories can ingest the models created by these tools and integrate the imported Metadata into the 
repository. Modeling tools are often the source of data dictionary content. 
1.3.5.13 Reference Data Repositories 
Reference Data documents the business values and descriptions of the various types of enumerated data 
(domains) and their contextual use in a system. Tools used to manage Reference Data are also capable of 
managing relationships between the various codified values within the same or across domains. These suites of 
tools normally provide capabilities to send the collected Reference Data to a Metadata repository, which in turn 
will provide mechanisms to associate the Reference Data to the business glossary and to the locations where it 
is physically implemented like columns or fields.  
1.3.5.14 Service Registries 
A service registry manages and stores the technical information about services and service end-points from a 
service oriented architecture (SOA) perspective. For example, definitions, interfaces, operations, input and 
output parameters, policies, versions, and sample usage scenarios. Some of the most important Metadata related 
to services includes service version, location of service, data center, availability, deployment date, service port, 
IP address, stats port, connection timeout, and connection retry timeout. Service registries can be interrogated to 
satisfy various needs like displaying a list of all available services, services with a specific version, obsolete 
services, or details about a specific service. Services can also be reviewed for potential re-use. The information 
contained in these repositories provides important facts on what data exists and how it moves between various 
systems or applications. Metadata in service repositories can be extracted and incorporated with Metadata 
collected from other tools to provide a complete picture of how data is moving between the various systems. 
1.3.5.15 Other Metadata Stores 
Other Metadata stores include specialized lists such as event registries, source lists or interfaces, code sets, 
lexicons, spatial and temporal schema, spatial reference, and distribution of digital geographic data sets, 
repositories of repositories, and business rules. 
 

