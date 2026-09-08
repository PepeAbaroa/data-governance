# página 392 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

388 • DMBOK2 
Figure 80 The Corporate Information Factory 
1.3.6 Dimensional DW (Kimball) 
Kimball’s Dimensional Data Warehouse is the other primary pattern for DW development. Kimball defines a 
data warehouse simply as “a copy of transaction data specifically structured for query and analysis” (Kimball, 
2002). The ‘copy’ is not exact, however. Warehouse data is stored in a dimensional data model. The 
dimensional model is designed to enable data consumers to understand and use the data, while also enabling 
query performance.65 It is not normalized in the way an entity relationship model is.  
Often referred to as Star Schema, dimensional models are comprised facts, which contain quantitative data 
about business processes (e.g., sales numbers), and dimensions, which store descriptive attributes related to fact 
data and allow data consumers to answer questions about the facts (e.g., how many units of product X were sold 
this quarter?) A fact table joins with many dimension tables, and when viewed as a diagram, appears as a star. 
(See Chapter 5.) Multiple fact tables will share the common, or conformed, dimensions via a ‘bus’, similar to a 
bus in a computer.66 Multiple data marts can be integrated at an enterprise level by plugging into the bus of 
conformed dimensions. 
The DW bus matrix shows the intersection of business processes that generate fact data and data subject areas 
that represent dimensions. Opportunities for conformed dimensions exist where multiple processes use the same 
data. Table 27 is a sample bus matrix. In this example, the business processes for Sales, Inventory, and Orders 
65 http://bit.ly/1udtNC8. 
66 The term bus came from Kimball’s electrical engineering background, where a bus was something providing common 
power to a number of electrical components. 
Reference Data
DM
DM
DM
DW
Op DM
ODS
App
App
App
App
Analysis*
Historical 
Reference Data
Operational Reports 
(per App)
Operational Reports 
(integrated)
Integration & Transformation
Raw Detailed Data
Exploratory 
Analysis*
Operational 
Analysis
Applications
Data Marts
 

[49 imágenes en esta página]
