# página 374 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

370 • DMBOK2 
consistent source of Master Data. However, it is costly to remove the functionality to update Master 
Data from existing systems of record. Business rules are implemented in a single system: the Hub.  
•
A Consolidated approach is a hybrid of Registry and Transaction Hub. The systems of record manage
Master Data local to their applications. Master Data is consolidated within a common repository and
made available from a data-sharing hub, the system of reference for Master Data. This eliminates the
need to access directly from the systems of record. The Consolidated approach provides an enterprise
view with limited impact on systems of record. However, it entails replication of data and there will be
latency between the hub and the systems of record.
Figure 77 Master Data Sharing Architecture Example 
2. Activities
As emphasized in Section 1.3.1, Master Data and Reference Data share certain characteristics (they are shared 
resources that provide context and meaning for other data and should be managed at the enterprise level), but 
they also differ in important ways (Reference Data sets are smaller, less volatile, do not require matching, 
merging, and linking, etc.). The activities section will first describe activities associated with MDM, and then 
describe those related to Reference Data. 
ODS
DW
(local)
MDS
App
App
App
App
App
App
DM
External
Partners
External
Partners
LZ
LDS
(optional)
DM
DW
(enterprise)
MDS
LDS
ODS
DW
App
LZ
DM
Cloud 
Environment
Master Data Hub
Environment
B2B Environment
Master Data 
Sharing Hub
Local Data 
Sharing Hub
Operational 
Data Store
Data 
Warehouse
Application 
Solution
Landing 
Zone
Data Mart
 

[34 imágenes en esta página]
