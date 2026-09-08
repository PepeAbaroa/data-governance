# página 116 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

112 • DMBOK2 
describes how the target architecture will become reality. The Enterprise Data Architecture roadmap must be 
integrated into an overall enterprise architecture roadmap that includes high-level milestones, resources needed, 
and costs estimations, divided in business capability work streams. The roadmap should be guided by a data 
management maturity assessment. (See Chapter 15.)  
Most business capabilities require data as an input; others also produce data on which other business capabilities 
are dependent. The enterprise architecture and the Enterprise Data Architecture can be formed coherently by 
resolving this data flow in a chain of dependencies between business capabilities. 
A business-data-driven roadmap starts with the business capabilities that are most independent (i.e., have the 
least dependency from other activities), and ends with those who are most dependent on others. Dealing with 
each business capability in sequence will follow an overall business data origination order. Figure 27 shows an 
example chain of dependency, with the lowest dependency at the top. Product Management and Customer 
Management do not depend on anything else and thus constitute Master Data. The highest dependency items are 
on the bottom where Customer’s Invoice Management depends on Customer Management and Sales Order 
Management, which in turn depends on two others.  
Figure 27 The Data Dependencies of Business Capabilities 
Product 
Management
Product Part 
Management
Sales Item 
Management
Sales Order 
Management
Customer 
Management
Customer’s 
Invoice 
Management
Production Order 
Management
Assembly 
Structure 
Management
Product 
Data
Product 
Data
BOM
Details
BOM
Details
Assembly
Structure
Data
Sales Order
Data
Sales Order
Data
Customer 
Data
Customer 
Data
Sales Item
Data

[25 imágenes en esta página]
