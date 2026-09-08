# página 376 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

372 • DMBOK2 
that can be compared to an organization’s internal data to improve contact information, addresses, and names 
(see Chapter 10). In addition to assessing the quality of existing data, it also necessary to understand the 
technology that supports the collection of inputs to an MDM effort. Existing technology will influence the 
architectural approach to MDM.  
2.1.3 Define Architectural Approach 
The architectural approach to MDM depends on business strategy, the platforms of existing data sources, and 
the data itself, particularly its lineage and volatility, and the implications of high or low latency. Architecture 
must account for data consumption and sharing models. Tooling for maintenance depends on both business 
requirements and architecture options. Tooling helps define and is dependent on the approach to stewardship 
and maintenance.  
The number of source systems to be integrated into the Master Data solution and the platforms of those systems 
need to be accounted for when determining the approach to integration. The size and geographic spread of an 
organization will also influence the integration approach. Small organizations may effectively utilize a 
transaction hub whereas a global organization with multiple systems is more likely to utilize a registry. An 
organization with ‘siloed’ business units and various source systems may decide that a consolidated approach is 
the correct path to follow. Business domain experts, Data Architects, and Enterprise Architects should provide 
perspective on approach. 
The data sharing hub architecture is particularly useful when there is no clear system of record for Master Data. 
In this case, multiple systems supply data. New data or updates from one system can be reconciled with data 
already supplied by another system. The data-sharing hub becomes the source of Master Data content for data 
warehouses or marts, reducing the complexity of extracts and the processing time for data transformation, 
remediation, and reconciliation. Of course, data warehouses must reflect changes made to the data-sharing hub 
for historical purposes, while the data-sharing hub itself may need to reflect just the current state.  
2.1.4 Model Master Data 
Master Data Management is a data integration process. To achieve consistent results and to manage the 
integration of new sources as an organization expands, it is necessary to model the data within subject areas. A 
logical or canonical model can be defined over the subject areas within the data-sharing hub. This would allow 
establishment of enterprise level definitions of subject area entities and attributes. (See Chapters 5 and 8.)  
2.1.5 Define Stewardship and Maintenance Processes 
Technical solutions can do remarkable work matching, merging, and managing identifiers for master records. 
However, the process also requires stewardship, not only to address records that fall out of the process, but also 
to remediate and improve the processes that cause them to fall out in the first place. MDM projects should 
 

