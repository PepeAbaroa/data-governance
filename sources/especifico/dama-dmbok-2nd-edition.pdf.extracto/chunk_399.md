# página 400 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

396 • DMBOK2 
2.2.2 Define DW/BI Management Processes 
Address production management with a coordinated and integrated maintenance process, delivering regular 
releases to the business community.  
It is crucial to establish a standard release plan (see Section 2.6). Ideally, the warehouse project team should 
manage each update to the deployed data product as a software release that provisions additional functionality. 
Establishing a schedule for releases allows for an annual demand and resource plan and standard delivery 
schedule. Use the internal release to tweak this standardized schedule, the resource expectations and estimate 
sheets derived for it. 
Establishing a functioning release process ensures that management understands this to be a data product-
centric proactive process and not an installed product addressed through reactive issue resolution. It is critical to 
work pro-actively and collaboratively in a cross-functional team to continuously grow and enhancement 
features – reactive support systems reduce adoption. 
2.3 Develop the Data Warehouse and Data Marts 
Typically, DW/BI projects have three concurrent development tracks: 
•
Data: The data necessary to support the analysis the business wants to do. This track involves
identifying the best sources for the data and designing rules for how the data is remediated,
transformed, integrated, stored, and made available for use by the applications. This step also includes
deciding how to handle data that doesn’t fit expectations.
•
Technology: The back-end systems and processes supporting the data storage and movement.
Integration with the existing enterprise is fundamental, as the warehouse is not an island unto itself.
Enterprise Architectures, specifically Technology and Application specialties, usually manage this
track.
•
Business Intelligence tools: The suite of applications necessary for data consumers to gain meaningful
insight from deployed data products.
2.3.1 Map Sources to Targets 
Source-to-target mapping establishes transformation rules for entities and data elements from individual sources 
to a target system. Such mapping also documents lineage for each data element available in the BI environment 
back to its respective source(s). 
The most difficult part of any mapping effort is determining valid links or equivalencies between data elements 
in multiple systems. Consider the effort to consolidate data into a DW from multiple billing or order 
 

