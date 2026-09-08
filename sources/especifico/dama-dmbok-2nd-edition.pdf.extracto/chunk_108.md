# página 109 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA ARCHITECTURE • 105 
These two types of specifications need to fit well together. As mentioned, both need to be reflected in current 
state and target state (architecture perspective), and also in transition state (project perspective). 
1.3.3.1 Enterprise Data Model 
Some organizations create an EDM as a stand-alone artifact. In other organizations, it is understood as 
composed of data models from different perspectives and at different levels of detail, that consistently describe 
an organization’s understanding of data entities, data attributes, and their relationships across the enterprise. An 
EDM includes both universal (Enterprise-wide Conceptual and Logical Models) and application- or project-
specific data models, along with definitions, specifications, mappings, and business rules.  
Adopting an industry standard model can jumpstart the process of developing an EDM. These models provide a 
useful guide and references. However, even if an organization starts with a purchased data model, producing 
enterprise-wide data models requires a significant investment. Work includes defining and documenting an 
organization’s vocabulary, business rules, and business knowledge. Maintaining and enriching an EDM requires 
an ongoing commitment of time and effort. 
An organization that recognizes the need for an enterprise data model must decide how much time and effort it 
can devote to building and maintaining it. EDMs can be built at different levels of detail, so resource 
availability will influence initial scope. Over time, as the needs of the enterprise demand, the scope and level of 
detail captured within an enterprise data model typically expands. Most successful enterprise data models are 
built incrementally and iteratively, using layers. Figure 23 shows how different types of models are related and 
how conceptual models are ultimately linkable to physical application data models. It distinguishes:  
•
A conceptual overview over the enterprise’s subject areas
•
Views of entities and relationships for each subject area
•
Detailed, partially attributed logical views of these same subject areas
•
Logical and physical models specific to an application or project
All levels are part of the Enterprise Data Model, and linkages create paths to trace an entity from top to bottom 
and between models in the same level. 
•
Vertical: Models in each level map to models in other levels. Model lineage is created using these
maps. For example, a table or file MobileDevice in a project-specific physical model may link to a
MobileDevice entity in the project-specific logical model, a MobileDevice entity in the Product subject
area in the Enterprise Logical Model, a Product conceptual entity in the Product Subject Area Model,
and to the Product entity in the Enterprise Conceptual Model.
•
Horizontal: Entities and relationships may appear in multiple models in the same level; entities in
logical models centered on one topic may relate to entities in other topics, marked or noted as external
to the subject area on the model images. A Product Part entity may appear in the Product subject area
models and in the Sales Order, Inventory, and Marketing subject areas, related as external links.

