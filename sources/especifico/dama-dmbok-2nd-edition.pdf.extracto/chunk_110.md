# página 111 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA ARCHITECTURE • 107 
approaches is usually recommended; starting with bottom-up using existing models and completing the 
enterprise data model by populating the models by delegating Subject Area modeling to projects. 
Figure 24 Subject Area Models Diagram Example 
The Subject Area discriminator (i.e., the principles that form the Subject Area structure) must be consistent 
throughout the enterprise data model. Frequently used subject area discriminator principles include: using 
normalization rules, dividing Subject Areas from systems portfolios (i.e., funding), forming Subject Areas from 
data governance structure and data ownership (organizational), using top-level processes (based on the business 
value chains), or using business capabilities (enterprise architecture-based). The Subject Area structure is 
usually most effective for Data Architecture work if it is formed using normalization rules. The normalization 
process will establish the major entities that carry/constitute each Subject Area. 
1.3.3.2 Data Flow Design 
Data flows are a type of data lineage documentation that depicts how data moves through business processes 
and systems. End-to-end data flows illustrate where the data originated, where it is stored and used, and how it 
is transformed as it moves inside and between diverse processes and systems. Data lineage analysis can help 
explain the state of data at a given point in the data flow. 
Product 
Platform
Product
Product 
Part
Market 
Offering
Portfolio
Sales 
Item
Sales Bundle
Bill-of-material 
(BOM)
Sales 
Order
Sales 
Order Item
Product Group
Part
Structure
Product Design 
Bill-of-material 
(BOM)
Belongs to
Uses
Offering Range
Occurs in
Specifies
Details
Product Design 
 Subject Area
Commercial 
Offer Subject 
Area
Sales  Subject 
Area
Sales 
Order Item 
Configuration

[3 imágenes en esta página]
