# página 354 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

350 • DMBOK2 
•
Lowering the cost and reducing the complexity of data usage and integration through standards,
common data models, and integration patterns
Reference and Master Data Management follow these guiding principles: 
•
Shared Data: Reference and Master Data must be managed so that they are shareable across the
organization.
•
Ownership: Reference and Master Data belong to the organization, not to a particular application or
department. Because they are widely shared, they require a high level of stewardship.
•
Quality: Reference and Master Data Management require ongoing Data Quality monitoring and
governance.
•
Stewardship: Business Data Stewards are accountable for controlling and ensuring the quality of
Reference Data.
•
Controlled Change:
o
At a given point of time, Master Data values should represent the organization’s best
understanding of what is accurate and current. Matching rules that change values should be
applied with caution and oversight. Any identifier merged or split should be reversible.
o
Changes to Reference Data values should follow a defined process; changes should be
approved and communicated before they are implemented.
•
Authority: Master Data values should be replicated only from the system of record. A system of
reference may be required to enable sharing of Master Data across an organization.
1.3 Essential Concepts 
1.3.1 Differences Between Master and Reference Data 
Different types of data play different roles within an organization. They also have different management 
requirements. A distinction is often made between Transaction and Master Data, as well as between Master 
Data and Reference Data. Malcolm Chisholm has proposed a six-layer taxonomy of data that includes 
Metadata, Reference Data, enterprise structure data, transaction structure data, transaction activity data, and 
transaction audit data (Chisholm, 2008; Talburt and Zhou, 2015). Within this taxonomy, he defines Master Data 
as an aggregation of Reference Data, enterprise structure data, and transaction structure data:  
•
Reference Data, for example, code and description tables, is data that is used solely to characterize
other data in an organization, or solely to relate data in a database to information beyond the
boundaries of the organization.
 

