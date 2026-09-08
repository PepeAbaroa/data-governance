# página 138 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

134 • DMBOK2 
A compound key is a set of two or more attributes that together uniquely identify an entity instance. Examples 
are US phone number (area code + exchange + local number) and credit card number (issuer ID + account ID + 
check digit). 
A composite key contains one compound key and at least one other simple or compound key or non-key 
attribute. An example is a key on a multi-dimensional fact table, which may contain several compound keys, 
simple keys, and optionally a load timestamp. 
1.3.3.3.2.2 Function-type Keys 
A super key is any set of attributes that uniquely identify an entity instance. A candidate key is a minimal set of 
one or more attributes (i.e., a simple or compound key) that identifies the entity instance to which it belongs. 
Minimal means that no subset of the candidate key uniquely identifies the entity instance. An entity may have 
multiple candidate keys. Examples of candidate keys for a customer entity are email address, cell phone 
number, and customer account number. Candidate keys can be business keys (sometimes called natural keys). A 
business key is one or more attributes that a business professional would use to retrieve a single entity instance. 
Business keys and surrogate keys are mutually exclusive. 
A primary key is the candidate key that is chosen to be the unique identifier for an entity. Even though an entity 
may contain more than one candidate key, only one candidate key can serve as the primary key for an entity. An 
alternate key is a candidate key that although unique, was not chosen as the primary key. An alternate key can 
still be used to find specific entity instances. Often the primary key is a surrogate key and the alternate keys are 
business keys. 
1.3.3.3.2.3 Identifying vs. Non-Identifying Relationships 
An independent entity is one where the primary key contains only attributes that belong to that entity. A 
dependent entity is one where the primary key contains at least one attribute from another entity. In relational 
schemes, most notations depict independent entities on the data modeling diagram as rectangles and dependent 
entities as rectangles with rounded corners.  
In the student example shown in Figure 38, Student and Course are independent entities and Registration is a 
dependent entity.  
Figure 38 Dependent and Independent Entity 
Registration
Student Number (FK)
Course Code (FK)
Registration Date
Course
Course Code
Course Name
Student
Student Number
Student First Name
Student Last Name
Student Birth Date
Have registered
Register
 

