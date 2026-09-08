# página 395 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA WAREHOUSING AND BUSINESS INTELLIGENCE • 391 
Figure 82 Conceptual DW/BI and Big Data Architecture 
1.3.7.3 Data Storage Areas 
The warehouse has a set of storage areas: 
•
Staging area: A staging area is an intermediate data store between an original data source and the
centralized data repository. Data is staged so that it can be transformed, integrated, and prepped for
loading to the warehouse.
•
Reference and Master Data conformed dimensions: Reference and Master Data may be stored in
separate repositories. The data warehouse feeds new Master Data and is fed by conformed dimension
contents from the separate repositories.
•
Central Warehouse: Once transformed and prepped, the DW data usually persists in the central or
atomic layer. This layer maintains all historical atomic data as well as the latest instance of the batch
run. The data structure of this area is developed and influenced based on performance needs and use
patterns. Several design elements are brought to bear:
o
The relationship between the business key and surrogate keys for performance
o
Creation of indices and foreign keys to support dimensions
o
Change Data Capture (CDC) techniques that are used to detect, maintain, and store history
© DATALEADERS.ORG
Report   Interact
Compare Evaluate
Predict Learn
Data Visualization
DaaS
Big Data 
Results
MDM
Reference & 
Master Data 
Conformed
Dimensions
Data Warehouse
Data Mastering
Data Quality Intervention
Enrichment & Augmentation
Sources
BI
Conceptual DW/BI and Big Data Architecture
Application
Operational
Reporting
Big Data
Data & Text Mining
Unstructured 
Analytics
Predictive Analytics
Machine Learning
Opertional Reporting 
& Analyics
Geospatial and 
Demographic Analytics
Performance 
Management
Cubes
ODS
Data Mart
Dependent
Data Stores
Evaluate
Model
Explore
Integrate
Ingest
Data Lake
Email
Multimedia
Sensors
IoT
Sociel Network
Web DaaS
DW
Operational
Systems
Central Warehouse
Subject-Oriented
Non-Volatile   
Time-Variant
Atomic
Historical Data
Staging Area
Clean
Integrate
Enrich
Standardize
 

[52 imágenes en esta página]
