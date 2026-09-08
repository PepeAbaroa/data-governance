# página 160 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

156 • DMBOK2 
attribute called phone number divides into several logical attributes for phone type code (home, office, fax, 
mobile, etc.), country code, (1 for US and Canada), area code, prefix, base phone number, and extension. 
2.2.1.2.5 Assign Domains 
Domains, which were discussed in Section 1.3.3.4, allow for consistency in format and value sets within and 
across projects. Student Tuition Amount and Instructor Salary Amount can both be assigned the Amount 
domain, for example, which will be a standard currency domain. 
2.2.1.2.6 Assign Keys 
Attributes assigned to entities are either key or non-key attributes. A key attribute helps identify one unique 
entity instance from all others, either fully (by itself) or partially (in combination with other key elements). 
Non-key attributes describe the entity instance but do not help uniquely identify it. Identify primary and 
alternate keys.  
2.2.1.3 Physical Data Modeling 
Logical data models require modifications and adaptations in order to have the resulting design perform well 
within storage applications. For example, changes required to accommodate Microsoft Access would be 
different from changes required to accommodate Teradata. Going forward, the term table will be used to refer 
to tables, files, and schemas; the term column to refer to columns, fields, and elements; and the term row to refer 
to rows, records, or instances. 
2.2.1.3.1 Resolve Logical Abstractions 
Logical abstraction entities (supertypes and subtypes) become separate objects in the physical database design 
using one of two methods. 
•
Subtype absorption: The subtype entity attributes are included as nullable columns into a table
representing the supertype entity.
•
Supertype partition: The supertype entity’s attributes are included in separate tables created for each
subtype.
2.2.1.3.2 Add Attribute Details 
Add details to the physical model, such as the technical name of each table and column (relational databases), or 
file and field (non-relational databases), or schema and element (XML databases). 
 

