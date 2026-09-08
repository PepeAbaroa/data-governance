# página 394 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

390 • DMBOK2 
Figure 81 Kimball's Data Warehouse Chess Pieces67 
Figure 82 also depicts aspects of the data lifecycle. Data moves from source systems, into a staging area where 
it may be cleansed and enriched as it is integrated and stored in the DW and/or an ODS. From the DW it may be 
accessed via marts or cubes and used for various kinds of reporting. Big Data goes through a similar process, 
but with a significant difference: while most warehouses integrate data before landing it in tables, Big Data 
solutions ingest data before integrating it. Big Data BI may include predictive analytics and data mining, as well 
as more traditional forms of reporting. (See Chapter 14.)  
1.3.7.1 Source Systems 
Source Systems, on the left side of Figure 82, include the operational systems and external data to be brought 
into the DW/BI environment. These typically include operational systems such as CRM, Accounting, and 
Human Resources applications, as well as operational systems that differ based on industry. Data from vendors 
and external sources may also be included, as may DaaS, web content, and any Big Data computation results.  
1.3.7.2 Data Integration 
Data integration covers Extract, Transform, and Load (ETL), data virtualization, and other techniques of getting 
data into a common form and location. In a SOA environment, the data services layers are part of this 
component. In Figure 82, all the arrows represent data integration processes. (See Chapter 8.) 
67 Adapted from Kimball and Ross (2002). Used with permission. 
Operational 
Source 
Systems
Data Staging 
Area
Data 
Presentation 
Area
Data  Access 
Tools
Extract
Extract
Extract
Extract
Load
Load
Load
Load
Data Mart #1
Data Mart #2
Data Mart #N
Access
Access
Access
Access
SERVICES:

Clean

Combine

Standardize

Conform 
Dimensions
REPORT 
WRITERS
ANALYTICAL 
APPLICATIONS
MODELS:
Forecasting
Scoring
Data Mining
AD-HOC
QUERIES
DATA STORE:

Flat Files 

Relational Tables

XML Datasets
PROCESSING:

Sorting

Sequencing
NO QUERIES
DW BUS 
Conformed Dimensions 
 

[3 imágenes en esta página]
