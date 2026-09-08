# página 176 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

172 • DMBOK2 
•
Set expectations for the DBA role in project work: Ensuring project methodology includes
onboarding the DBA in project definition phase can help throughout the SDLC. The DBA can
understand project needs and support requirements up-front. This will improve communication by
clarifying the project team’s expectations from the data group. Having a dedicated primary and
secondary DBA during analysis and design clarify expectations about DBA tasks, standards, work
effort, and timelines for development work. Teams should also clarify expectations for support after
implementation.
1.3 Essential Concepts 
1.3.1 Database Terms 
Database terminology is specific and technical. In working as a DBA or with DBAs, it is important to 
understand the specifics of this technical language:  
•
Database: Any collection of stored data, regardless of structure or content. Some large databases refer
to instances and schema.
•
Instance: An execution of database software controlling access to a certain area of storage. An
organization will usually have multiple instances executing concurrently, using different areas of
storage. Each instance is independent of all other instances.
•
Schema: A subset of a database objects contained within the database or an instance. Schemas are
used to organize objects into more manageable parts. Usually, a schema has an owner and an access
list particular to the schema’s contents. Common uses of schemas are to isolate objects containing
sensitive data from the general user base, or to isolate read-only views from the underlying tables in
relational databases. Schema can also be used to refer to a collection of database structures with
something in common.
•
Node: An individual computer hosting either processing or data as part of a distributed database.
•
Database abstraction means that a common application interface (API) is used to call database
functions, such that an application can connect to multiple different databases without the programmer
having to know all function calls for all possible databases. ODBC (Open Database Connectivity) is an
example of an API that enables database abstraction. Advantages include portability; disadvantages
include inability to use specific database functions that are not common across databases.
1.3.2 Data Lifecycle Management 
DBAs maintain and assure the accuracy and consistency of data over its entire lifecycle through the design, 
implementation, and usage of any system that stores, processes, or retrieves data. The DBA is the custodian of 
all database changes. While many parties may request changes, the DBA defines the precise changes to make to 
the database, implements the changes, and controls the changes.  
 

