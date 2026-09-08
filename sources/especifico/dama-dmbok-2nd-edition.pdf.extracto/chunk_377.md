# página 378 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

374 • DMBOK2 
2.2.3 Define Architectural Approach 
Before purchasing or building a tool to manage Reference Data, it is critical to account for requirements and for 
the challenges posed by the Reference Data to be managed. For example, the volatility of data (most Reference 
Data is relatively static, but some is quite volatile), the frequency of updates, and the consumption models. 
Determine whether it is required to keep historical data on changes to the values or the definitions of the values. 
If the organization will purchase data from a vendor, account for the delivery and integration method.  
The architectural approach needs to recognize that, invariably, some Reference Data will need to be updated 
manually. Ensure that the interface for updates is straightforward and can be configured to enforce basic data 
entry rules, such as ensuring parent/child relationships are maintained in Reference Data that includes 
hierarchies. The RDM tool should enable Stewards to make ad hoc updates without the need for technical 
support and should include workflows to ensure approvals and notifications are automated. Data Stewards 
should schedule known updates to align with the publication of new codes. Data consumers should be informed 
of all changes. In cases where Reference Data drives programming logic, the potential impact of changes should 
be assessed and accounted for before the changes are introduced.  
2.2.4 Model Reference Data Sets 
Many people think of Reference Data as simply codes and descriptions. However, much Reference Data is more 
complicated than that. For example, a ZIP Code data set will usually include information on state and county, as 
well as other geo-political attributes. For purposes of enabling long-term usage and establishing accurate 
Metadata, as well as for the maintenance process itself, it is valuable to create data models of Reference Data 
sets. Models help data consumers understand the relationships within the Reference Data set and they can be 
used to establish data quality rules.  
2.2.5 Define Stewardship and Maintenance Processes 
Reference Data requires stewardship to ensure that values are complete and current and that definitions are clear 
and understandable. In some cases, stewards will be directly responsible for hands-on maintenance of Reference 
Data; in other cases, they may facilitate the process. For example, if several different business units require 
Reference Data to support the same concept, a steward may facilitate discussions that define common values in 
a crosswalk.  
As part of the stewardship process, it is helpful to capture basic Metadata about each Reference Data set. This 
could include: steward name, originating organization, expected frequency of updates, schedule for updates, 
processes using the Reference Data, whether historical versions of the data need to be retained, and more (see 
Section 1.3.2.6). Documenting what processes use Reference Data will enable more effective communication 
regarding changes to the data.  
 

