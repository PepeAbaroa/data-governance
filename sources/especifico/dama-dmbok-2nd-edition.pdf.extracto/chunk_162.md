# página 163 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 159 
2.4 Maintain the Data Models 
Once the data models are built, they need to be kept current. Updates to the data model need to be made when 
requirements change and frequently when business processes change. Within a specific project, often when one 
model level needs to change, a corresponding higher level of model needs to change. For example, if a new 
column is added to a physical data model, that column frequently needs to be added as an attribute to the 
corresponding logical data model. A good practice at the end of each development iteration is to reverse 
engineer the latest physical data model and make sure it is still consistent with its corresponding logical data 
model. Many data modeling tools help automate this process of comparing physical with logical. 
3. Tools
There are many types of tools that can assist data modelers in completing their work, including data modeling, 
lineage, data profiling tools, and Metadata repositories. 
3.1 Data Modeling Tools 
Data modeling tools are software that automate many of the tasks the data modeler performs. Entry-level data 
modeling tools provide basic drawing functionality including a data modeling pallet so that the user can easily 
create entities and relationships. These entry-level tools also support rubber banding, which is the automatic 
redrawing of relationship lines when entities are moved. More sophisticated data modeling tools support 
forward engineering from conceptual to logical to physical to database structures, allowing the generation of 
database data definition language (DDL). Most will also support reverse engineering from database up to 
conceptual data model. These more sophisticated tools often support functionality such as naming standards 
validation, spellcheckers, a place to store Metadata (e.g., definitions and lineage), and sharing features (such as 
publishing to the Web). 
3.2 Lineage Tools 
A lineage tool is software that allows the capture and maintenance of the source structures for each attribute on 
the data model. These tools enable impact analysis; that is, one can use them to see if a change in one system or 
part of system has effects in another system. For example, the attribute Gross Sales Amount might be sourced 
from several applications and require a calculation to populate – lineage tools would store this information. 
Microsoft Excel® is a frequently-used lineage tool. Although easy to use and relatively inexpensive, Excel does 
not enable real impact analysis and leads to manually managing Metadata. Lineage is also frequently captured 
in a data modeling tool, Metadata repository, or data integration tool. (See Chapters 11 and 12.) 
 

