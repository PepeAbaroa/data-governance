# página 108 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

104 • DMBOK2 
•
The architect perspective (business logic): System logical models detailing system requirements and
unconstrained design represented by Architects as Designers in representation models.
•
The engineer perspective (business physics): Physical models optimizing the design for
implementation for specific use under the constraints of specific technology, people, costs, and
timeframes specified by Engineers as Builders in specification models.
•
The technician perspective (component assemblies): A technology-specific, out-of-context view of
how components are assembled and operate configured by Technicians as Implementers in
configuration models.
•
The user perspective (operations classes): Actual functioning instances used by Workers as
Participants. There are no models in this perspective.
As noted previously, each cell in the Zachman Framework represents a unique type of design artifact, defined 
by the intersection of its row and column. Each artifact represents how the specific perspective answers the 
fundamental questions. 
1.3.3 Enterprise Data Architecture 
Enterprise Data Architecture defines standard terms and designs for the elements that are important to the 
organization. The design of an Enterprise Data Architecture includes depiction of the business data as such, 
including the collection, storage, integration, movement, and distribution of data.  
As data flows in an organization through feeds or interfaces, it is secured, integrated, stored, recorded, 
catalogued, shared, reported on, analyzed, and delivered to stakeholders. Along the way, the data may be 
verified, enhanced, linked, certified, aggregated, anonymized, and used for analytics until archived or purged. 
The Enterprise Data Architecture descriptions must therefore include both Enterprise Data Models (e.g., data 
structures and data specifications), as well as Data Flow Design: 
•
Enterprise Data Model (EDM): The EDM is a holistic, enterprise-level, implementation-independent
conceptual or logical data model providing a common consistent view of data across the enterprise. It
is common to use the term to mean a high-level, simplified data model, but that is a question of
abstraction for presentation. An EDM includes key enterprise data entities (i.e., business concepts),
their relationships, critical guiding business rules, and some critical attributes. It sets forth the
foundation for all data and data-related projects. Any project-level data model must be based on the
EDM. The EDM should be reviewed by stakeholders, so that there is consensus that it effectively
represents the enterprise.
•
Data Flow Design: Defines the requirements and master blueprint for storage and processing across
databases, applications, platforms, and networks (the components). These data flows map the
movement of data to business processes, locations, business roles, and to technical components.

