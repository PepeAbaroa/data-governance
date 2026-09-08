# página 410 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

406 • DMBOK2 
Conceptually, this illustrates as a cube. Multi-dimensional analysis with cubes is particularly useful where there 
are well-known ways analysts want to look at summaries of data. 
A traditional application is financial analysis, where analysts want to repeatedly traverse known hierarchies to 
analyze data; for example, date (such as Year, Quarter, Month, Week, Day), organization (such as Region, 
Country, Business Unit, Department), and product hierarchy (such as Product Category, Product Line, Product). 
Many tools today embed OLAP cubes into their software footprint and some even seamlessly automate and 
integrate the definition and population process. This means that any user in any business process can slice and 
dice their data. Align this capability with the power users in the subject area communities and deliver it along a 
self-service channel empowering these selected users to analyze their data their way. 
Typically, OLAP tools have both a server component and an end user client-facing component installed on the 
desktop, or available on the web. Some desktop components are accessible from within a spreadsheet appearing 
as an embedded menu or function item. The architecture selected (ROLAP, MOLAP, HOLAP) will guide the 
development efforts but common to all will be definition of cube structure, aggregate needs, Metadata 
augmentation and analysis of data sparsity.  
Structuring the cube to provision desired functional requirements may require splitting larger dimensions into 
separate cubes to accommodate storage, population, or calculation requirements. Use levels of aggregation to 
ensure calculation and retrieval of desired formulas occurs within agreed upon response times. End user 
augmentation of hierarchies enable fulfillment the aggregation, calculation, or population requirements. In 
addition, sparsity of cube data may require addition or removal of aggregate structures or refine materialization 
needs in the warehouse data layer provisioning it. 
Provisioning role-based security or multi-language text within the cube may require extra dimensions, 
additional functions, calculations, or sometimes creating separate cube structures. Striking a balance between 
end user flexibility, performance, and server workloads means some negotiating is to be expected. The 
negotiation typically occurs during the loading processes and may require hierarchy changes, aggregate 
structure changes or additional warehouse materialized data objects. Strike the right balance among cube count, 
server workload, and delivered flexibility, so that the refresh occurs in a timely manner, and cubes provide 
reliable and consistent queries without high storage or server utilization costs.  
The value of On Line Analytical Processing (OLAP) Tools and cubes is reduction of the chance of confusion 
and erroneous interpretation, by aligning the data content with the analyst’s mental model. The analyst can 
navigate through the database and screen for a particular subset of the data, changing the data’s orientation and 
defining analytical calculations. Slice-and-dice is the user-initiated process of navigation by calling for page 
displays interactively, through the specification of slices via rotations and drill down / up. Common OLAP 
operations include slice and dice, drill down, drill up, roll up, and pivot. 
•
Slice: A slice is a subset of a multi-dimensional array corresponding to a single value for one or more
members of the dimensions not in the subset.
•
Dice: The dice operation is a slice on more than two dimensions of a data cube, or more than two
consecutive slices.
 

