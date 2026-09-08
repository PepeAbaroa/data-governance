# página 153 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 149 
Figure 51 Dimensional Physical Data Model 
1.3.5.3.2 Views 
A view is a virtual table. Views provide a means to look at data from one or many tables that contain or 
reference the actual attributes. A standard view runs SQL to retrieve data at the point when an attribute in the 
view is requested. An instantiated (often called ‘materialized’) view runs at a predetermined time. Views are 
used to simplify queries, control data access, and rename columns, without the redundancy and loss of 
referential integrity due to denormalization. 
1.3.5.3.3 Partitioning 
Partitioning refers to the process of splitting a table. It is performed to facilitate archiving and to improve 
retrieval performance. Partitioning can be either vertical (separating groups of columns) or horizontal 
(separating groups of rows). 
•
Vertically split: To reduce query sets, create subset tables that contain subsets of columns. For
example, split a customer table in two based on whether the fields are mostly static or mostly volatile
(to improve load / index performance), or based on whether the fields are commonly or uncommonly
included in queries (to improve table scan performance).
 

[1 imágenes en esta página]
