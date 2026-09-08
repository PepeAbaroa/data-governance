# página 413 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA WAREHOUSING AND BUSINESS INTELLIGENCE • 409 
•
Define data sensitivity and security constraints
•
Perform tool selection
•
Secure resources
•
Create an ingestion process to evaluate and receive source data
Identify and inventory sensitive or restricted data elements in the warehouse. This data will need to be masked 
or obfuscated to prevent access by unauthorized personnel. Additional constraints may apply when considering 
outsourcing for implementation or maintenance activities.  
Account for security constrains before selecting tools and assigning resources. Ensure data governance 
processes for review and approval have been followed. DW/BI projects risk refocus or total cancellation due to 
these overarching factors.  
5.2 Release Roadmap 
Because they require a large development effort, warehouses are built incrementally. Whatever method chosen 
to implement, be it waterfall, iterative or agile, it should account for the desired end state. That is why a 
roadmap is a valuable planning tool. The method combined with the maintenance processes can be both flexible 
and adaptive to balance the pressures of individual project delivery with overall goals of re-usable data and 
infrastructure.  
An incremental approach leveraging the DW bus matrix as a communication and marketing tool is suggested. 
Use business-determined priorities tethered by exposure metrics to determine how much rigor and overhead to 
apply to each increment; a small single-sourced delivery may afford rule relaxation especially when limited 
exposure is felt should those issues be realized by the organization. 
Each increment will modify existing capabilities or add brand new capabilities typically aligned with a newly 
onboarded business unit. Apply a consistent needs and abilities process to determine the next business unit to 
onboard. Maintain a back-order or work item list to identify outstanding capabilities and the business-facing 
priorities. Determine any technical dependencies that require delivery in a different order. Then package this 
work into a software release. Each release can be delivered at an agreed-upon pace: quarterly, monthly, weekly, 
or even faster when appropriate. Manage the releases with the business partners by assembling a roadmap: a 
listing of releases by date by capabilities. 
5.3 Configuration Management 
Configuration management aligns with the release roadmap and provides the necessary back office stitching and 
scripts to automate development, testing, and transportation to production. It also brands the model by the 
release at the database level, and ties the codebase to that brand in an automated manner so that manually 
 

