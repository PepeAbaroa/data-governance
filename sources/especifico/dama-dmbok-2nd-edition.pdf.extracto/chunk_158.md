# página 159 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 155 
Requirements analysis includes the elicitation, organization, documentation, review, refinement, approval, and 
change control of business requirements. Some of these requirements identify business needs for data and 
information. Express requirement specifications in both words and diagrams. 
Logical data modeling is an important means of expressing business data requirements. For many people, as the 
old saying goes, ‘a picture is worth a thousand words’. However, some people do not relate easily to pictures; 
they relate better to reports and tables created by data modeling tools.  
Many organizations have formal requirements. Management may guide drafting and refining formal 
requirement statements, such as “The system shall…” Written data requirement specification documents may be 
maintained using requirements management tools. The specifications gathered through the contents of any such 
documentation should carefully synchronize with the requirements captured with data models to facilitate 
impact analysis so one can answer questions like “Which parts of my data models represent or implement 
Requirement X?” or “Why is this entity here?” 
2.2.1.2.2 Analyze Existing Documentation 
It can often be a great jump-start to use pre-existing data artifacts, including already built data models and 
databases. Even if the data models are out-of-date, parts can be useful to start a new model. Make sure however, 
that any work done based on existing artifacts is validated by the SMEs for accuracy and currency. Companies 
often use packaged applications, such as Enterprise Resource Planning (ERP) systems, that have their own data 
models. Creation of the LDM should take into account these data models and either use them, where applicable, 
or map them to the new enterprise data model. In addition, there could be useful data modeling patterns, such as 
a standard way of modeling the Party Role concept. Numerous industry data models capture how a generic 
industry, such as retail or manufacturing, should be modeled. These patterns or industry data models can then be 
customized to work for the particular project or initiative. 
2.2.1.2.3 Add Associative Entities 
Associative entities are used to describe Many-to-Many (or Many-to-Many-to-Many, etc.) relationships. An 
associative entity takes the identifying attributes from the entities involved in the relationship, and puts them 
into a new entity that just describes the relationship between the entities. This allows the addition of attributes to 
describe that relationship, like in effective and expiration dates. Associative entities may have more than two 
parents. Associative entities may become nodes in graph databases. In dimensional modeling, associative 
entities usually become fact tables. 
2.2.1.2.4 Add Attributes  
Add attributes to the conceptual entities. An attribute in a logical data model should be atomic. It should contain 
one and only one piece of data (fact) that cannot be divided into smaller pieces. For example, a conceptual 
 

