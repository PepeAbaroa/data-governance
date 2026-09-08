# página 447 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

METADATA MANAGEMENT • 443 
•
Business focus: Limit the lineage discovery to data elements prioritized by the business. Start from the
target locations and trace back to the source systems where the specific data originates. By limiting the
scanned assets to those that move, transfer, or update the selected data elements, this approach will
enable business data consumers to understand what is happening to the specific data element as it
moves through systems. If coupled with data quality measurements, lineage can be used to pinpoint
where system design adversely impacts the quality of the data.
•
Technical focus: Start at the source systems and identify all the immediate consumers, then identify all
the subsequent consumers of the first set identified and keep repeating these steps until all systems are
identified. Technology users benefit more from the system discovery strategy in order to help answer
the various questions about the data. This approach will enable technology and business users to
answer question about discovering data elements across the enterprise, like “Where is social security
number?” or generate impact reports like “What systems are impacted if the width of a specific column
is changed?” This strategy can, however, be complex to manage.
Many data integration tools offer lineage analysis that considers not only the developed population code but the 
data model and the physical database as well. Some offer business user facing web interfaces to monitor and 
update definitions. These begin to look like business glossaries.  
Documented lineage helps both business and technical people use data. Without it, much time is wasted in 
investigating anomalies, potential change impacts, or unknown results. Look to implement an integrated impact 
and lineage tool that can understand all the moving parts involved in the load process as well as end user 
reporting and analytics. Impact reports outline which components are affected by a potential change expediting 
and streamlining estimating and maintenance tasks. 
4.2 Metadata for Big Data Ingest 
Many data management professionals are familiar and comfortable with structured data stores, where every 
item can be clearly identified and tagged. Nowadays, though, much data comes in less structured formats. Some 
unstructured sources will be internal to the organization, and some will be external. In either case, there is no 
longer a need to physically bring the data to one place. Through the new technologies, the program will go to 
the data as opposed to moving the data to the program, reducing the amount of data movement, and speeding up 
the execution of the process. Nevertheless, successful data management in a data lake depends on managing 
Metadata.  
Metadata tags should be applied to data upon ingestion. Metadata then can be used to identify data content 
available for access in the data lake. Many ingestion engines profile data as it is ingested. Data profiling can 
identify data domains, relationships, and data quality issues. It can also enable tagging. On ingestion, Metadata 
tags can be added to identify sensitive or private (like Personally Identifiable Information – PPI) data, for 
example. Data scientists may add confidence, textual identifiers, and codes representing behavior clusters. (See 
Chapter 14.) 
 

