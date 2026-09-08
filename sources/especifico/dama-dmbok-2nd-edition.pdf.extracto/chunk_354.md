# página 355 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

REFERENCE AND MASTER DATA • 351 
•
Enterprise Structure Data, for example, a chart of accounts, enables reporting of business activity by
business responsibility.
•
Transaction Structure Data, for example customer identifiers, describes the things must be present
for a transaction to occur: products, customers, vendors.
Chisholm’s definition distinguishes Master Data from transaction activity data that records details about 
transactions, and from transaction audit data that describes the state of transactions, as well as from Metadata, 
which describes other data (Chisholm, 2008). In this respect, Chisholm’s definition is similar to the DAMA 
Dictionary’s definition: Master Data is “the data that provides the context for business activity data in the form 
of common and abstract concepts that relate to the activity. It includes the details (definitions and identifiers) of 
internal and external objects involved in business transactions, such as customers, products, employees, 
vendors, and controlled domains (code values)” (DAMA, 2009). 
Many people understand Master Data to include both transaction structure data and enterprise structure data. 
David Loshin’s definition of Master Data aligns largely with these types. He describes Master Data objects as 
core business objects used in different applications across an organization, along with their associated Metadata, 
attributes, definitions, roles, connections, and taxonomies. Master Data objects represent those ‘things’ that 
matter most to an organization – those that are logged in transactions, reported on, measured, analyzed (Loshin, 
2008). 
Master Data requires identifying and / or developing a trusted version of truth for each instance of conceptual 
entities such as product, place, account, person, or organization and maintaining the currency of that version. 
The primary challenge with Master Data is entity resolution (also called identity management), the process of 
discerning and managing associations between data from different systems and processes. The entity instances 
represented by Master Data rows will be represented differently across systems. Master Data Management 
works to resolve these differences in order to consistently identify individual entity instances (i.e., specific 
customers, products, etc.) in different contexts. This process must also be managed over time, so that the 
identifiers for these Master Data entity instances remain consistent.56 
Reference Data and Master Data share conceptually similar purposes. Both provide context critical to the 
creation and use of transactional data. (Reference Data also provides context for Master Data.) They enable data 
to be meaningfully understood. Importantly, both are shared resources that should be managed at the enterprise 
level. Having multiple instances of the same Reference Data is inefficient and inevitably leads to inconsistency 
between them. Inconsistency leads to ambiguity, and ambiguity introduces risk to an organization. A successful 
Reference Data or Master Data Management program involves the full range of data management functions 
(Data Governance, Data Quality, Metadata Management, Data Integration, etc.).  
Reference Data also has characteristics that distinguish it from other kinds of Master Data (e.g., enterprise and 
transactional structure data). It is less volatile. Reference Data sets are generally less complex and smaller than 
56 John Talburt and Yinle Zhou (2015) describe the two step process in ER: first, determine whether two records refer to the 
same entity, then merge and reconcile data in the records in order to create a master record. They refer to Entity Identity 
Information Management (EIIM) as the process of ensuring that “an entity under management in the MDM system is 
consistently labeled with the same unique identifier from process to process.”  
 

