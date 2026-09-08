# página 380 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

376 • DMBOK2 
4.1 Adhere to Master Data Architecture 
Establishing and following proper reference architecture is critical to managing and sharing Master Data across 
an organization. The integration approach should take into account the organizational structure of the business, 
the number of distinct systems of record, the data governance implementation, the importance of access and 
latency of data values, and the number of consuming systems and applications. 
4.2 Monitor Data Movement 
Data integration processes for Master and Reference Data should be designed to ensure timely extraction and 
distribution of data across the organization. As data flows within a Reference or Master Data sharing 
environment, data flow should be monitored in order to:  
•
Show how data is shared and used across the organization
•
Identify data lineage from / to administrative systems and applications
•
Assist root cause analysis of issues
•
Show effectiveness of data ingestion and consumption integration techniques
•
Denote latency of data values from source systems through consumption
•
Determine validity of business rules and transformations executed within integration components
4.3 Manage Reference Data Change 
Since Reference Data is a shared resource, it cannot be changed arbitrarily. The key to successful Reference 
Data Management is organizational willingness to relinquish local control of shared data. To sustain this 
support, provide channels to receive and respond to requests for changes to Reference Data. The Data 
Governance Council should ensure that policies and procedures are implemented to handle changes to data 
within reference and Master Data environments.  
Changes to Reference Data will need to be managed. Minor changes may affect a few rows of data. For 
example, when the Soviet Union broke into independent states, the term Soviet Union was deprecated and new 
codes were added. In the healthcare industry, procedure and diagnosis codes are updated annually to account for 
refinement of existing codes, obsoleting of codes, and the introduction of new codes. Major revisions to 
Reference Data impact data structure. For example, ICD-10 Diagnostic Codes are structured in ways very 
different from ICD-9. ICD10 has a different format. There are different values for the same concepts. More 
importantly, ICD-10 has additional principles of organization. ICD10 codes have a different granularity and are 
much more specific, so more information is conveyed in a single code. Consequently, there are many more of 
them (as of 2015, there were 68,000 ICD-10 codes, compared with 13,000 ICD-9s).62  
62 http://bit.ly/1SSpds9 (accessed 8/13/16). 
 

