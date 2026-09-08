# página 433 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

METADATA MANAGEMENT • 429 
and many other operational Metadata attributes. The most common form of database is relational. Relational 
databases manage the data as a set of tables and columns, where a table contains one or more columns, indexes, 
constraints, views, and procedures. A Metadata solution should be able to connect to the various databases and 
data sets and read all of the Metadata exposed by the database. Some of the Metadata repository tools can 
integrate the exposed Metadata from the system management tools to provide a more holistic picture about the 
captured physical assets. 
1.3.5.8 Data Mapping Management Tools 
Mapping management tools are used during the analysis and design phase of a project to transform 
requirements into mapping specifications, which can then be consumed directly by a data integration tool or 
used by the developers to generate data integration code. Mapping documentation is also often held in excel 
documents across the enterprise. Vendors are now considering centralized repositories for the mapping 
specifications with capabilities to perform version control and change analysis between versions. Many 
mapping tools integrate with data integration tools to automate the generation of the data integration programs 
and most can exchange data with other Metadata and Reference Data repositories. (See Chapter 8.) 
1.3.5.9 Data Quality Tools 
Data quality tools assess the quality of data through validation rules. Most of these tools provide the capability 
to exchange the quality scores and profiles patterns with other Metadata repositories, enabling the Metadata 
repository to attach the quality scores to the relevant physical assets. 
1.3.5.10 Directories and Catalogs 
While data dictionaries and glossaries contain detailed information about terminology, tables, and fields, a 
directory or catalog contains information about systems, sources, and locations of data within an organization. 
A directory of Metadata is particularly useful to developers and data super users, such as data stewardship teams 
and data analysts, to understand the scope of data in the enterprise, whether to research issues or to find 
information about sourcing new applications.  
1.3.5.11 Event Messaging Tools 
Event messaging tools move data between diverse systems. To do so, they require a lot of Metadata. They also 
generate Metadata that describes this movement. These tools include graphic interfaces through which they 
manage the logic of data movement. They can export the interfaces implementation details, movement logic, 
and processing statistics to other Metadata repositories.  
 

