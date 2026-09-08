# página 356 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

352 • DMBOK2 
either Transactional or Master Data sets. They have fewer columns and fewer rows. The challenges of entity 
resolution are not part of Reference Data Management.  
The focus of data management differs between Reference and Master Data: 
•
Master Data Management (MDM) entails control over Master Data values and identifiers that enable
consistent use, across systems, of the most accurate and timely data about essential business entities.
The goals of MDM include ensuring availability of accurate, current values while reducing risks
associated with ambiguous identifiers (those identified with more than one instance of an entity and
those that refer to more than one entity).
•
Reference Data Management (RDM) entails control over defined domain values and their
definitions. The goal of RDM is to ensure the organization has access to a complete set of accurate and
current values for each concept represented.
One challenge of Reference Data Management is that of ownership or responsibility for definition and 
maintenance. Some Reference Data originates outside of the organizations that use it. Some crosses internal 
organizational boundaries and may not be owned by a single department. Other Reference Data may be created 
and maintained within a department but have potential value elsewhere in an organization. Determining 
responsibility for obtaining data and managing updates is part of RDM. Lack of accountability introduces risk, 
as differences in Reference Data may cause misunderstanding of data context (as when two business units have 
different values to classify the same concept).  
Because Master and Reference Data provide context for transactions, they shape the Transaction data entering 
an organization during operations (for example, in CRM and ERP systems). They also frame analysis 
performed on Transaction Data.  
1.3.2 Reference Data 
As noted, Reference Data is any data used to characterize or classify other data, or to relate data to information 
external to an organization (Chisholm, 2001). The most basic Reference Data consists of codes and 
descriptions, but some Reference Data can be more complex and incorporate mappings and hierarchies. 
Reference Data exists in virtually every data store. Classifications and categories may include statuses or types 
(e.g., Order Status: New, In Progress, Closed, Cancelled). External information may include geographic or 
standards information (e.g., Country Code: DE, US, TR).  
Reference Data may be stored in different ways to meet the different needs. For example, data integration (e.g., 
data mappings for standardization or data quality checks), or other application functionality (e.g., synonym 
rings to enable search and discovery). It may also have device specific user interface considerations (e.g., 
multiple languages). Common storage techniques use: 
•
Code tables in relational databases, linked via foreign keys to other tables to maintain referential
integrity functions within the database management system
 

