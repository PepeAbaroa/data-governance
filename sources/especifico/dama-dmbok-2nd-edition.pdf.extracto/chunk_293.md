# página 294 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

290 • DMBOK2 
2.2.1.1 Select Interaction Model 
Determine which interaction model or combination will fulfill the requirements – hub-and-spoke, point-to-
point, or publish-subscribe. If the requirements match an existing interaction pattern already implemented, re-
use the existing system as much as possible, to reduce development efforts. 
2.2.1.2 Design Data Services or Exchange Patterns 
Create or re-use existing integration flows to move the data. These data services should be companions to 
existing similar data services, but be careful to not create multiple almost-identical services, as troubleshooting 
and support increasingly become difficult if services proliferate. If an existing data flow can be modified to 
support multiple needs, it may be worthwhile to make that change instead of creating a new service. 
Any data exchange specification design should start with industry standards, or other exchange patterns already 
existing. When possible, make any changes to existing patterns generic enough to be useful to other systems; 
having specific exchange patterns that only relate to one exchange has the same issues as point-to-point 
connections.  
2.2.2 Model Data Hubs, Interfaces, Messages, and Data Services 
Data structures needed in Data Integration and Interoperability include those in which data persists, such as 
Master Data Management hubs, data warehouses and marts, and operational data stores, and those that are 
transient and used only for moving or transforming data, such as interfaces, message layouts, and canonical 
models. Both types should be modeled. (See Chapter 5.) 
2.2.3 Map Data Sources to Targets 
Almost all data integration solutions include transforming data from source to target structures. Mapping 
sources to targets involves specifying the rules for transforming data from one location and format to another. 
For each attribute mapped, a mapping specification  
•
Indicates the technical format of the source and target
•
Specifies transformations required for all intermediate staging points between source and target
•
Describes how each attribute in a final or intermediate target data store will be populated
•
Describes whether data values need to be transformed; for example, by looking up the source value in
a table that indicates the appropriate target value
•
Describes what calculations are required
 

