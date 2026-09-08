# página 165 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 161 
reference for an organization’s in-progress efforts to help the modelers make models that are more complete. In 
others, it can merely save the data modeler some data entry effort for annotated common elements.  
4. Best Practices
4.1 Best Practices in Naming Conventions 
The ISO 11179 Metadata Registry, an international standard for representing Metadata in an organization, 
contains several sections related to data standards, including naming attributes and writing definitions. 
Data modeling and database design standards serve as the guiding principles to effectively meet business data 
needs, conform to Enterprise and Data Architecture (see Chapter 4) and ensure the quality of data (see Chapter 
14). Data architects, data analysts, and database administrators must jointly develop these standards. They must 
complement and not conflict with related IT standards. 
Publish data model and database naming standards for each type of modeling object and database object. 
Naming standards are particularly important for entities, tables, attributes, keys, views, and indexes. Names 
should be unique and as descriptive as possible. 
Logical names should be meaningful to business users, using full words as much as possible and avoiding all 
but the most familiar abbreviations. Physical names must conform to the maximum length allowed by the 
DBMS, so use abbreviations where necessary. While logical names use blank spaces as separators between 
words, physical names typically use underscores as word separators. 
Naming standards should minimize name changes across environments. Names should not reflect their specific 
environment, such as test, QA, or production. Class words, which are the last terms in attribute names such as 
Quantity, Name, and Code, can be used to distinguish attributes from entities and column names from table 
names. They can also show which attributes and columns are quantitative rather than qualitative, which can be 
important when analyzing the contents of those columns. 
4.2 Best Practices in Database Design 
In designing and building the database, the DBA should keep the following design principles in mind 
(remember the acronym PRISM): 
•
Performance and ease of use: Ensure quick and easy access to data by approved users in a usable and
business-relevant form, maximizing the business value of both applications and data.
 

