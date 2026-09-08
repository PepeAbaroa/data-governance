# página 393 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA WAREHOUSING AND BUSINESS INTELLIGENCE • 389 
all require Date and Product data. Sales and Inventory both require Store data, while Inventory and Orders 
require Vendor data. Date, Product, Store and Vendor are all candidates for conformed dimensions. In contrast, 
Warehouse is not shared; it is used only by Inventory. 
Table 27 DW-Bus Matrix Example 
Subject Areas 
Business Processes 
Date 
Product 
Store 
Vendor 
Warehouse 
Sales 
X 
X 
X 
Inventory 
X 
X 
X 
X 
X 
Orders 
X 
X 
X 
Conformed Dimension Candidate 
Yes 
Yes 
Yes 
Yes 
No 
The enterprise DW bus matrix can be used to represent the long-term data content requirements for the DW/BI 
system, independent of technology. This tool enables an organization to scope manageable development efforts. 
Each implementation builds an increment of the overall architecture. At some point, enough dimensional 
schemas exist to make good on the promise of an integrated enterprise data warehouse environment. 
Figure 81 represents Kimball’s Data Warehouse Chess Pieces view of DW/BI architecture. Note that Kimball’s 
Data Warehouse is more expansive than Inmon’s. The DW encompasses all components in the data staging and 
data presentation areas. 
•
Operational source systems: Operational / transactional applications of the Enterprise. These create
the data that is integrated into the ODS and DW. This component is equivalent to the application
systems in the CIF diagram.
•
Data staging area: Kimball’s staging includes the set of processes needed to integrate and transform
data for presentation. It can be compared to a combination of CIF’s integration, transformation, and
DW components. Kimball’s focus is on efficient end-delivery of the analytical data, a scope smaller
than Inmon’s corporate management of data. Kimball’s enterprise DW can fit into the architecture of
the data staging area.
•
Data presentation area: Similar to the Data Marts in the CIF. The key architectural difference being
an integrating paradigm of a ‘DW Bus,’ such as shared or conformed dimensions unifying the multiple
data marts.
•
Data access tools: Kimball’s approach focuses on end users’ data requirements. These needs drive the
adoption of appropriate data access tools.
1.3.7 DW Architecture Components 
The data warehouse environment includes a collection of architectural components that need to be organized to 
meet the needs of the enterprise. Figure 82 depicts the architectural components of the DW/BI and Big Data 
Environment discussed in this section. The evolution of Big Data has changed the DW/BI landscape by adding 
another path through which data may be brought into an enterprise.  
 

