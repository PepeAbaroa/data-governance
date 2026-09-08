# página 167 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 163 
•
A list and description of standard data modeling and database design deliverables
•
A list of standard names, acceptable abbreviations, and abbreviation rules for uncommon words, that
apply to all data model objects
•
A list of standard naming formats for all data model objects, including attribute and column class
words
•
A list and description of standard methods for creating and maintaining these deliverables
•
A list and description of data modeling and database design roles and responsibilities
•
A list and description of all Metadata properties captured in data modeling and database design,
including both business Metadata and technical Metadata. For example, guidelines may set the
expectation that the data model captures lineage for each attribute.
•
Metadata quality expectations and requirements (see Chapter 13)
•
Guidelines for how to use data modeling tools
•
Guidelines for preparing for and leading design reviews
•
Guidelines for versioning of data models
•
Practices that are discouraged
5.1.2 Review Data Model and Database Design Quality 
Project teams should conduct requirements reviews and design reviews of the  conceptual data model, logical 
data model, and physical database design. The agenda for review meetings should include items for reviewing 
the starting model (if any), the changes made to the model and any other options that were considered and 
rejected, and how well the new model conforms to any modeling or architecture standards in place. 
Conduct design reviews with a group of subject matter experts representing different backgrounds, skills, 
expectations, and opinions. It may require executive mandate to get expert resources allocated to these reviews. 
Participants must be able to discuss different viewpoints and reach group consensus without personal conflict, 
as all participants share the common goal of promoting the most practical, best performing and most usable 
design. Chair each design review with one leader who facilitates the meeting. The leader creates and follows an 
agenda, ensures all required documentation is available and distributed, solicits input from all participants, 
maintains order and keeps the meeting moving, and summarizes the group’s consensus findings. Many design 
reviews also use a scribe to capture points of discussion. 
In reviews where there is no approval, the modeler must rework the design to resolve the issues. If there are 
issues that the modeler cannot resolve on their own, the final say should be given by the owner of the system 
reflected by the model. 
5.1.3 Manage Data Model Versioning and Integration 
Data models and other design specifications require careful change control, just like requirements specifications 
and other SDLC deliverables. Note each change to a data model to preserve the lineage of changes over time. If 
 

