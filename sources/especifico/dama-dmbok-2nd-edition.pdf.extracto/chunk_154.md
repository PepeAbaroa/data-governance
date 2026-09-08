# página 155 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 151 
comprises a separate normal form, and each successive level does not need to include previous levels. 
Normalization levels include: 
•
First normal form (1NF): Ensures each entity has a valid primary key, and every attribute depends on
the primary key; removes repeating groups, and ensures each attribute is atomic (not multi-valued).
1NF includes the resolution of many-to-many relationships with an additional entity often called an
associative entity.
•
Second normal form (2NF): Ensures each entity has the minimal primary key and that every attribute
depends on the complete primary key.
•
Third normal form (3NF): Ensures each entity has no hidden primary keys and that each attribute
depends on no attributes outside the key (“the key, the whole key and nothing but the key”).
•
Boyce / Codd normal form (BCNF): Resolves overlapping composite candidate keys. A candidate
key is either a primary or an alternate key. ‘Composite’ means more than one (i.e., two or more
attributes in an entity’s primary or alternate keys), and ‘overlapping’ means there are hidden business
rules between the keys.
•
Fourth normal form (4NF): Resolves all many-to-many-to-many relationships (and beyond) in pairs
until they cannot be broken down into any smaller pieces.
•
Fifth normal form (5NF): Resolves inter-entity dependencies into basic pairs, and all join
dependencies use parts of primary keys.
The term normalized model usually means the data is in 3NF. Situations requiring BCNF, 4NF, and 5NF occur 
rarely.  
1.3.7 Abstraction 
Abstraction is the removal of details in such a way as to broaden applicability to a wide class of situations while 
preserving the important properties and essential nature from concepts or subjects. An example of abstraction is 
the Party/Role structure, which can be used to capture how people and organizations play certain roles (e.g., 
employee and customer). Not all modelers or developers are comfortable with, or have the ability to work with 
abstraction. The modeler needs to weigh the cost of developing and maintaining an abstract structure versus the 
amount of rework required if the unabstracted structure needs to be modified in the future (Giles 2011). 
Abstraction includes generalization and specialization. Generalization groups the common attributes and 
relationships of entities into supertype entities, while specialization separates distinguishing attributes within an 
entity into subtype entities. This specialization is usually based on attribute values within an entity instance. 
Subtypes can also be created using roles or classification to separate instances of an entity into groups by 
function. An example is Party, which can have subtypes of Individual and Organization. 
 

