# página 162 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

158 • DMBOK2 
select and define appropriate indexes for database tables. Major RDBMS products support many types of 
indexes. Indexes can be unique or non-unique, clustered or non-clustered, partitioned or non-partitioned, single 
column or multi-column, b-tree or bitmap or hashed. Without an appropriate index, the DBMS will revert to 
reading every row in the table (table scan) to retrieve any data. On large tables, this is very costly. Try to build 
indexes on large tables to support the most frequently run queries, using the most frequently referenced 
columns, particularly keys (primary, alternate, and foreign). 
2.2.1.3.7 Partition for Performance 
Great consideration must be given to the partitioning strategy of the overall data model (dimensional) especially 
when facts contain many optional dimensional keys (sparse). Ideally, partitioning on a date key is 
recommended; when this is not possible, a study is required based on profiled results and workload analysis to 
propose and refine the subsequent partitioning model.  
2.2.1.3.8 Create Views 
Views can be used to control access to certain data elements, or to embed common join conditions or filters to 
standardize common objects or queries. Views themselves should be requirements-driven. In many cases, they 
will need to be developed via a process that mirrors the development of the LDM and PDM.  
2.2.2 Reverse Engineering 
Reverse engineering is the process of documenting an existing database. The PDM is completed first to 
understand the technical design of an existing system, followed by an LDM to document the business solution 
that the existing system meets, followed by the CDM to document the scope and key terminology within the 
existing system. Most data modeling tools support reverse engineering from a variety of databases; however, 
creating a readable layout of the model elements still requires a modeler. There are several common layouts 
(orthogonal, dimensional, and hierarchical) which can be selected to get the process started, but contextual 
organization (grouping entities by subject area or function) is still largely a manual process. 
2.3 Review the Data Models 
As do other areas of IT, models require quality control. Continuous improvement practices should be employed. 
Techniques such as time-to-value, support costs, and data model quality validators such as the Data Model 
Scorecard® (Hoberman, 2009), can all be used to evaluate the model for correctness, completeness, and 
consistency. Once the CDM, LDM, and PDM are complete, they become very useful tools for any roles that 
need to understand the model, ranging from business analysts through developers.  
 

