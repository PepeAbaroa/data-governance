# página 161 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 157 
Define the physical domain, physical data type, and length of each column or field. Add appropriate constraints 
(e.g., nullability and default values) for columns or fields, especially for NOT NULL constraints. 
2.2.1.3.3 Add Reference Data Objects 
Small Reference Data value sets in the logical data model can be implemented in a physical model in three 
common ways: 
•
Create a matching separate code table: Depending on the model, these can be unmanageably
numerous.
•
Create a master shared code table: For models with a large number of code tables, this can collapse
them into one table; however, this means that a change to one reference list will change the entire
table. Take care to avoid code value collisions as well.
•
Embed rules or valid codes into the appropriate object’s definition: Create a constraint in the
object definition code that embeds the rule or list. For code lists that are only used as reference for one
other object, this can be a good solution.
2.2.1.3.4 Assign Surrogate Keys 
Assign unique key values that are not visible to the business and have no meaning or relationship with the data 
with which they are matched. This is an optional step and depends primarily on whether the natural key is large, 
composite, and whose attributes are assigned values that could change over time. 
If a surrogate key is assigned to be the primary key of a table, make sure there is an alternate key on the original 
primary key. For example, if on the LDM the primary key for Student was Student First Name, Student Last 
Name, and Student Birth Date (i.e., a composite primary key), on the PDM the primary key for Student may 
be the surrogate key Student ID. In this case, there should be an alternate key defined on the original primary 
key of Student First Name, Student Last Name, and Student Birth Date. 
2.2.1.3.5 Denormalize for Performance 
In some circumstances, denormalizing or adding redundancy can improve performance so much that it 
outweighs the cost of the duplicate storage and synchronization processing. Dimensional structures are the main 
means of denormalization. 
2.2.1.3.6 Index for Performance  
An index is an alternate path for accessing data in the database to optimize query (data retrieval) performance. 
Indexing can improve query performance in many cases. The database administrator or database developer must 
 

