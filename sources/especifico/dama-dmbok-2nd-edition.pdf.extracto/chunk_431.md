# página 432 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

428 • DMBOK2 
1.3.5.5 Data Dictionaries 
A data dictionary defines the structure and contents of data sets, often for a single database, application, or 
warehouse. The dictionary can be used to manage the names, descriptions, structure, characteristics, storage 
requirements, default values, relationships, uniqueness, and other attributes of every data element in a model. It 
should also contain table or file definitions. Data dictionaries are embedded in database tools for the creation, 
operation, manipulation of data contained in them. To make this Metadata available to data consumers, it must 
be extracted from the database or modeling tools. Data dictionaries can also describe in business terminology 
what data elements are available to the community, provisioned under what security restrictions, and applied in 
which business process. Time can be saved when defining, publishing, and maintaining a semantic layer for 
reporting and analysis by leveraging the content directly from the logical model. However, as noted earlier, 
existing definitions should be used with caution, especially in an organization with a low level of maturity 
around Metadata management.  
Many key business processes, relationships, and terminologies are explained during the development of the data 
model. This information, captured in the logical data model, is often lost when physical structures are deployed 
to production. A data dictionary can help ensure that this information is not lost entirely to the organization and 
that the logical and physical models are kept in agreement after production deployment.  
1.3.5.6 Data Integration Tools 
Many data integration tools are used for executables to move data from one system to another or between 
various modules within the same system. Many of these tools generate transient files, which might contain 
copies or derived copies of the data. These tools are capable of loading data from various sources and then 
operating on the loaded data, through grouping, remediation, re-formatting, joining, filtering, or other 
operations, and then generating output data, which is distributed to the target locations. They document the 
lineage as data as it moves between systems. Any successful Metadata solution should be able to use the lineage 
Metadata as it is moves through the integration tools and expose it as a holistic lineage from the actual sources 
to the final destinations.  
Data integration tools provide application interfaces (API) to allow external Metadata repositories to extract the 
lineage information and the transient files Metadata. Once the Metadata repository collects the information, 
some tools can generate a holistic lineage diagram for any data element. Data integration tools also provide 
Metadata about the execution of the various data integration jobs, including last successful run, duration, and 
job status. Some Metadata repositories can extract the data integration runtime statistics and Metadata and 
expose it alongside the data elements. (See Chapters 6 and 8.) 
1.3.5.7 Database Management and System Catalogs 
Database catalogs are an important source of Metadata. They describe the content of databases, along with 
sizing information, software versions, deployment status, network uptime, infrastructure uptime, availability, 
 

