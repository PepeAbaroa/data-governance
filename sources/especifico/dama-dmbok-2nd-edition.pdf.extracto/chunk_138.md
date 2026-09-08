# página 139 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 135 
Dependent entities have at least one identifying relationship. An identifying relationship is one where the 
primary key of the parent (the entity on the one side of the relationship) is migrated as a foreign key to the 
child’s primary key, as can be seen with the relationship from Student to Registration, and from Course to 
Registration. In non-identifying relationships, the primary key of the parent is migrated as a non-primary 
foreign key attribute to the child. 
1.3.3.4 Domain 
In data modeling, a domain is the complete set of possible values that an attribute can be assigned. A domain 
may be articulated in different ways (see points at the end of this section). A domain provides a means of 
standardizing the characteristics of the attributes. For example, the domain Date, which contains all possible 
valid dates, can be assigned to any date attribute in a logical data model or date columns/fields in a physical 
data model, such as: 
•
EmployeeHireDate
•
OrderEntryDate
•
ClaimSubmitDate
•
CourseStartDate
All values inside the domain are valid values. Those outside the domain are referred to as invalid values. An 
attribute should not contain values outside of its assigned domain. EmployeeGenderCode, for example, may 
be limited to the domain of female and male. The domain for EmployeeHireDate may be defined simply as 
valid dates. Under this rule, the domain for EmployeeHireDate does not include February 30 of any year.  
One can restrict a domain with additional rules, called constraints. Rules can relate to format, logic, or both. For 
example, by restricting the EmployeeHireDate domain to dates earlier than today’s date, one would eliminate 
March 10, 2050 from the domain of valid values, even though it is a valid date. EmployeeHireDate could also 
be restricted to days in a typical workweek (e.g., dates that fall on a Monday, Tuesday, Wednesday, Thursday, 
or Friday).  
Domains can be defined in different ways. 
•
Data Type: Domains that specify the standard types of data one can have in an attribute assigned to
that domain. For example, Integer, Character(30), and Date are all data type domains.
•
Data Format: Domains that use patterns including templates and masks, such as are found in postal
codes and phone numbers, and character limitations (alphanumeric only, alphanumeric with certain
special characters allowed, etc.) to define valid values.
•
List: Domains that contain a finite set of values. These are familiar to many people from functionality
like dropdown lists. For example, the list domain for OrderStatusCode can restrict values to only
{Open, Shipped, Closed, Returned}.
 

