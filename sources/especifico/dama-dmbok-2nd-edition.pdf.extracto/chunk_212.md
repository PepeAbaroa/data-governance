# página 213 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 209 
Automated and manual data remediation is commonly performed in migration to improve the quality of data, 
eliminate redundant or obsolete information, and match the requirements of the new system. Data migration 
phases (design, extraction, remediation, load, verification) for applications of moderate to high complexity are 
commonly repeated several times before the new system is deployed. 
3. Tools
In addition to the database management systems themselves, DBAs use multiple other tools to manage 
databases. For example, modeling and other application development tools, interfaces that allow users to write 
and execute queries, data evaluation and modification tools for data quality improvement, and performance load 
monitoring tools.  
3.1 Data Modeling Tools 
Data modeling tools automate many of the tasks the data modeler performs. Some data modeling tools allow the 
generation of database data definition language (DDL). Most support reverse engineering from database into a 
data model. Tools that are more sophisticated validate naming standards, check spelling, store Metadata such as 
definitions and lineage, and even enable publishing to the web. (See Chapter 5.) 
3.2 Database Monitoring Tools 
Database monitoring tools automate monitoring of key metrics, such as capacity, availability, cache 
performance, user statistics, etc., and alert DBAs and NSAs to database issues. Most such tools can 
simultaneously monitor multiple database types.  
3.3 Database Management Tools 
Database systems have often included management tools. In addition, several third-party software packages 
allow DBAs to manage multiple databases. These applications include functions for configuration, installation 
of patches and upgrades, backup and restore, database cloning, test management, and data clean-up routines. 
3.4 Developer Support Tools 
Developer Support tools contain a visual interface for connecting to and executing commands on a database. 
Some are included with the database management software. Others include third-party applications. 
 

