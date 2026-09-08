# página 361 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

REFERENCE AND MASTER DATA • 357 
1.3.2.5 Computational Reference Data 
Many business activities rely on access to common, consistent calculations. For example, foreign exchange 
calculations rely on managed, time stamped exchange value tables. Computational Reference Data differs from 
other types because of the frequency with which it changes. Many organizations purchase this kind of data from 
third parties who ensure that it is complete and accurate. Attempting to maintain this data internally is likely to 
be fraught with latency issues. 
1.3.2.6 Standard Reference Data Set Metadata 
Reference Data, like other data, can change over time. Given its prevalence within any organization, it is 
important to maintain key Metadata about Reference Data sets to ensure their lineage and currency are 
understood and maintained. Table 23 provides examples of this Metadata. 
Table 23 Critical Reference Data Metadata Attributes 
Reference Data Set 
Key Information 
Description 
Formal Name 
Official, especially if external name of the Reference Data set (e.g., ISO 
3166-1991 Country Code List) 
Internal Name 
Name associated with the data set within the organization (e.g., Country 
Codes – ISO) 
Data Provider 
The party that provides and maintains the Reference Data set. This can 
be external (ISO), internal (a specific department), or external – 
extended (obtained from an external party but then extended and 
modified internally). 
Data Provider Data Set Source 
Description of where data provider’s data sets can be obtained. This is 
likely a Universal Resource Identifier (URI) within or outside of the 
enterprise network. 
Data Provider Latest Version 
Number 
If available and maintained, this describes the latest version of the 
external data provider’s data set where information may be added or 
deprecated from the version in the organization 
Data Provider Latest Version Date 
If available and maintained, this describes when the standard list was 
last updated 
Internal Version Number 
Version number of the current Reference Data set or version number of 
the last update that was applied against the data set 
Internal Version Reconciliation 
Date 
Date when data set was last updated based on the external source 
Internal Version Last Update Date 
Date data set was last changed. This does not mean reconciliation with 
an external version. 
1.3.3 Master Data 
Master Data is data about the business entities (e.g., employees, customers, products, financial structures, assets, 
and locations) that provide context for business transactions and analysis. An entity is a real world object 
(person, organization, place, or thing). Entities are represented by entity instances, in the form of data / records. 
 

