# página 527 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

BIG DATA AND DATA SCIENCE • 523 
5. Implementation Guidelines
Many of the general principles of managing warehouse data apply to managing Big Data: ensuring that the data 
sources are reliable, having sufficient Metadata to enable data use, managing the quality of data, figuring out 
how to integrate data from different sources, and ensuring that data is secure and protected. (See Chapters 6, 7, 
and 8.) The differences in implementing a Big Data environment are connected to a set of unknowns: how the 
data will be used, which data will be valuable, how long it needs to be retained. 
Data velocity may lead people to think they do not have time to implement controls. This is a dangerous 
assumption. With larger data sets, managing ingestion and inventorying data in a lake is critical to preventing it 
from becoming a swamp.  
Ingestion may not always require organizational ownership or commitment to the data set being studied. 
Consider leasing a Big Data platform for finite periods to explore data of interest. Exploration can quickly 
determine which areas show potential value. Do this before ingesting into the organizational data lake, data 
store, or data staging area; once landed, it can be awkward to remove. 
5.1 Strategy Alignment 
Any Big Data / Data Science program should be strategically aligned with organizational objectives. 
Establishing a Big Data strategy drives activities related to user community, data security, Metadata 
management, including lineage, and Data Quality Management.  
The strategy should document goals, approach, and governance principles. The ability to leverage Big Data 
requires building organizational skills and capabilities. Use capability management to align business and IT 
initiatives and project a roadmap. Strategy deliverables should account for managing:  
•
Information lifecycle
•
Metadata
•
Data quality
•
Data acquisition
•
Data access and security
•
Data governance
•
Data privacy
•
Learning and adoption
•
Operations
5.2 Readiness Assessment / Risk Assessment  
As with any development project, implementation of a Big Data or Data Science initiative should align with real 
business needs. Assess organizational readiness in relation to critical success factors: 
 

