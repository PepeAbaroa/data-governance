# página 365 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

REFERENCE AND MASTER DATA • 361 
should guide how applications are configured to take advantage of data reconciliation and data quality 
verification capabilities.  
Figure 76 Key Processing Steps for MDM 
1.3.3.4.1 Data Model Management 
Master Data work brings to light the importance of clear and consistent logical data definitions. The model 
should help the organization overcome ‘system speak’. Terms and definitions used within a source system may 
make sense within the confines of that system but they do not always make sense at an enterprise level. For 
Master Data, terms and definitions used at an enterprise level should be in context of the business conducted 
across the organization and not necessarily dependent on the source system contributing data values. 
For attributes that make up Master Data, the granularity of the definition and associated data values must also 
make sense across the organization. Source systems may present the identical attribute name but the data values 
are in completely different contexts at the enterprise level. Similarly, source systems may present differently 
named attributes that at the enterprise level coalesce to a single attribute and the data values are in the proper 
context. Sometimes multiple attributes are presented from a single source and their respective data values are 
used to derive a single data value for an attribute defined at the enterprise level. 
1.3.3.4.2 Data Acquisition 
Even within a given source, data representing the same entity instance can look different, as illustrated in Table 
24, where there are inconsistencies in how names, addresses, and telephone numbers are presented. This 
example will be referenced again later in the chapter.  
Table 24 Source Data as Received by the MDM System 
Source ID 
Name 
Address 
Telephone 
123 
John Smith 
123 Main, Dataland, SQ 98765 
234 
J. Smith 
123 Main, Dataland, DA 
2345678900 
345 
Jane Smith 
123 Main, Dataland, DA 
234-567-8900 
Data Model 
Management
Data Validation, 
Standardization, 
and Enrichment
Data Sharing & 
Stewardship
Data 
Acquisition
Entity 
Resolution
 

