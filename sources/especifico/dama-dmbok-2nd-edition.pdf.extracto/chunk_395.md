# página 396 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

392 • DMBOK2 
•
Operational Data Store (ODS): The ODS is a version of a central persisted store that supports lower
latencies, and therefore operational use. Since the ODS contains a time window of data and not the
history, it can be refreshed much more quickly than a warehouse. Sometimes real-time streams are
snapshotted at predefined intervals into the ODS to enable integrated reporting and analysis. Over
time, with the increasing frequency of updates driven by business needs, and growing technology and
techniques to integrate real-time data into the DW, many installations have merged their ODS into the
existing DW or Data Mart architecture.
•
Data marts: A data mart is a type of data store often used to support presentation layers of the data
warehouse environment. It is also used for presenting a departmental or functional sub-set of the DW
for integrated reporting, query, and analysis of historical information. The data mart is oriented to a
specific subject area, a single department, or a single business process. It can also form the basis of a
virtualized warehouse where the combined marts comprise the resulting warehouse entity. Data
integration processes will refresh, update or expand the contents of the various marts from the
persistence layer.
•
Cubes: Three classic implementation approaches support Online Analytical Processing (OLAP). Their
names relate to underlying database types, such as Relational, Multi-dimensional, and Hybrid.
1.3.8 Types of Load Processing 
Data warehousing involves two main types of data integration processes: historical loads and ongoing updates. 
Historical data is usually loaded only once, or a few times while working out data issues, and then never again. 
Ongoing updates are consistently scheduled and executed to keep the data in the warehouse up-to-date. 
1.3.8.1 Historical Data 
One advantage of a data warehouse is that it can capture detailed history of the data it stores. There are different 
methods to capture this detail. An organization that wants to capture history should design based on 
requirements. Being able to reproduce point-in-time snapshots requires a different approach than simply 
presenting current state. 
The Inmon data warehouse suggests that all data is stored in a single data warehouse layer. This layer will store 
cleansed, standardized, and governed atomic level data. A common integration and transformation layer 
facilitates reuse across the delivery implementations. An enterprise data model is required for success. Once 
validated, this single store is available to different data consumers via a star structured data mart. 
The Kimball data warehouse suggests that the data warehouse is composed of a combination of departmental 
data marts containing cleansed, standardized, and governed data. The data marts will store the history at the 
atomic level. Conformed dimensions and conformed facts will deliver enterprise level information.  
 

