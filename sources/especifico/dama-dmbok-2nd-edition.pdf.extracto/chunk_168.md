# página 169 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 165 
presents the Model Score for the category divided by the Total Score for the category. For example, receiving 
10 out of 15 would lead to 66%. The comments column should document information that explains the score in 
more detail or captures the action items required to fix the model. The last row contains the overall score 
assigned to the model, a sum of each of the columns.  
A brief description of each category follows: 
1.
How well does the model capture the requirements? Here we ensure that the data model represents
the requirements. If there is a requirement to capture order information, in this category we check the
model to make sure it captures order information. If there is a requirement to view Student Count by
Semester and Major, in this category we make sure the data model supports this query.
2.
How complete is the model? Here completeness means two things: completeness of requirements and
completeness of Metadata. Completeness of requirements means that each requirement that has been
requested appears on the model. It also means that the data model only contains what is being asked
for and nothing extra. It’s easy to add structures to the model anticipating that they will be used in the
near future; we note these sections of the model during the review. The project may become too hard
to deliver if the modeler includes something that was never asked for. We need to consider the likely
cost of including a future requirement in the case that it never eventuates. Completeness of Metadata
means that all of the descriptive information surrounding the model is present as well; for example, if
we are reviewing a physical data model, we would expect formatting and nullability to appear on the
data model.
3.
How well does the model match its scheme? Here we ensure that the model level of detail
(conceptual, logical, or physical), and the scheme (e.g., relational, dimensional, NoSQL) of the model
being reviewed matches the definition for this type of model.
4.
How structurally sound is the model? Here we validate the design practices employed to build the
model to ensure one can eventually build a database from the data model. This includes avoiding
design issues such as having two attributes with the same exact name in the same entity or having a
null attribute in a primary key.
5.
How well does the model leverage generic structures? Here we confirm an appropriate use of
abstraction. Going from Customer Location to a more generic Location, for example, allows the
design to more easily handle other types of locations such as warehouses and distribution centers.
6.
How well does the model follow naming standards? Here we ensure correct and consistent naming
standards have been applied to the data model. We focus on naming standard structure, term, and style.
Structure means that the proper building blocks are being used for entities, relationships, and attributes.
For example, a building block for an attribute would be the subject of the attribute such as ‘Customer’
or ‘Product’. Term means that the proper name is given to the attribute or entity. Term also includes
proper spelling and abbreviation. Style means that the appearance, such as upper case or camel case, is
consistent with standard practices.
 

