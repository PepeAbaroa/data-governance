# página 137 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 133 
Figure 36 Foreign Keys 
1.3.3.3 Attribute 
An attribute is a property that identifies, describes, or measures an entity. Attributes may have domains, which 
will be discussed in Section 1.3.3.4. The physical correspondent of an attribute in an entity is a column, field, 
tag, or node in a table, view, document, graph, or file.  
1.3.3.3.1 Graphic Representation of Attributes 
In data models, attributes are generally depicted as a list within the entity rectangle, as shown in Figure 37, 
where the attributes of the entity Student include Student Number, Student First Name, Student Last Name, 
and Student Birth Date.  
Figure 37 Attributes 
1.3.3.3.2 Identifiers 
An identifier (also called a key) is a set of one or more attributes that uniquely defines an instance of an entity. 
This section defines types of keys by construction (simple, compound, composite, surrogate) and function 
(candidate, primary, alternate).  
1.3.3.3.2.1 Construction-type Keys 
A simple key is one attribute that uniquely identifies an entity instance. Universal Product Codes (UPCs) and 
Vehicle Identification Numbers (VINs) are examples of simple keys. A surrogate key is also an example of a 
simple key. A surrogate key is a unique identifier for a table. Often a counter and always system-generated 
without intelligence, a surrogate key is an integer whose meaning is unrelated to its face value. (In other words, 
a Month Identifier of 1 cannot be assumed to represent January.) Surrogate keys serve technical functions and 
should not be visible to end users of a database. They remain behind the scenes to help maintain uniqueness, 
allow for more efficient navigation across structures, and facilitate integration across applications. 
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
Student
Student Number
Student First Name
Student Last Name
Student Birth Date
 

