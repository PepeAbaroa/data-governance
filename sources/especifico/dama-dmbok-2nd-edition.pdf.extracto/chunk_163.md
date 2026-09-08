# página 164 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

160 • DMBOK2 
3.3 Data Profiling Tools 
A data profiling tool can help explore the data content, validate it against existing Metadata, and identify Data 
Quality gaps/deficiencies, as well as deficiencies in existing data artifacts, such as logical and physical models, 
DDL, and model descriptions. For example, if the business expects that an Employee can have only one job 
position at a time, but the system shows Employees have more than one job position in the same timeframe, this 
will be logged as a data anomaly. (See Chapters 8 and 13.) 
3.4 Metadata Repositories 
A Metadata repository is a software tool that stores descriptive information about the data model, including the 
diagram and accompanying text such as definitions, along with Metadata imported from other tools and 
processes (software development and BPM tools, system catalogs, etc.). The repository itself should enable 
Metadata integration and exchange. Even more important than storing the Metadata is sharing the Metadata. 
Metadata repositories must have an easily accessible way for people to view and navigate the contents of the 
repository. Data modeling tools generally include a limited repository. (See Chapter 13.) 
3.5 Data Model Patterns 
Data model patterns are reusable modeling structures that can be applied to a wide class of situations. There are 
elementary, assembly, and integration data model patterns. Elementary patterns are the ‘nuts and bolts’ of data 
modeling. They include ways to resolve many-to-many relationships, and to construct self-referencing 
hierarchies. Assembly patterns represent the building blocks that span the business and data modeler worlds. 
Business people can understand them – assets, documents, people and organizations, and the like. Equally 
importantly, they are often the subject of published data model patterns that can give the modeler proven, 
robust, extensible, and implementable designs. Integration patterns provide the framework for linking the 
assembly patterns in common ways (Giles, 2011).  
3.6 Industry Data Models 
Industry data models are data models pre-built for an entire industry, such as healthcare, telecom, insurance, 
banking, or manufacturing. These models are often both broad in scope and very detailed. Some industry data 
models contain thousands of entities and attributes. Industry data models can be purchased through vendors or 
obtained through industry groups such as ARTS (for retail), SID (for communications), or ACORD (for 
insurance).  
Any purchased data model will need to be customized to fit an organization, as it will have been developed 
from multiple other organizations’ needs. The level of customization required will depend on how close the 
model is to an organization’s needs, and how detailed the most important parts are. In some cases, it can be a 
 

