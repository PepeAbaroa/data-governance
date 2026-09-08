# página 284 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

280 • DMBOK2 
system or organization exchanging data. Each system needs to transform data only to and from the central 
canonical model, rather than to the format of the multitude of systems with which it may want to exchange data. 
Although developing and agreeing on a shared message format is a major undertaking, having a canonical 
model can significantly reduce the complexity of data interoperability in an enterprise, and thus greatly lower 
the cost of support. The creation and management of the common canonical data model for all data interactions 
is a complex item of overhead that is required in the implementation of an enterprise data integration solution 
using a hub-and-spoke interaction model. It is justifiable in support of managing the data interactions between 
more than three systems and critical for managing data interactions in environments of more than 100 
application systems. 
1.3.6 Interaction Models 
Interaction models describe ways to make connections between systems in order to transfer data. 
1.3.6.1 Point-to-point 
The vast majority of interactions between systems that share data do so ‘point-to-point’; they pass data directly 
to each other. This model makes sense in the context of a small set of systems. However, it becomes quickly 
inefficient and increases organizational risk when many systems require the same data from the same sources.  
•
Impacts to processing: If source systems are operational, then the workload from supplying data
could affect processing.
•
Managing interfaces: The number of interfaces needed in a point-to-point interaction model
approaches the number of systems squared (s2). Once they are built, these interfaces need to be
maintained and supported. The workload to manage and support interfaces between the systems can
quickly become greater than supporting the systems themselves.
•
Potential for inconsistency: Design issues arise when multiple systems require different versions or
formats of the data. The use of multiple interfaces to obtain data will lead to inconsistencies in the data
sent to downstream systems.
1.3.6.2 Hub-and-spoke 
The hub-and-spoke model, an alternative to point-to-point, consolidates shared data (either physically or 
virtually) in a central data hub that many applications can use. All systems that want to exchange data do so 
through a central common data control system, rather than directly with one another (point-to-point). Data 
Warehouses, Data Marts, Operational Data Stores, and Master Data Management hubs are the most well-known 
examples of data hubs. 
 

