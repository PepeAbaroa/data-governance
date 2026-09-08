# página 144 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

140 • DMBOK2 
1.3.4.2.5 Conformed Dimensions 
Conformed dimensions are built with the entire organization in mind instead of just a particular project; this 
allows these dimensions to be shared across dimensional models, due to containing consistent terminology and 
values. For example, if Calendar is a conformed dimension, a dimensional model built to count student 
applicants by Semester will contain the same values and definition of Semester as a dimensional model built to 
count student graduates. 
1.3.4.2.6 Conformed Facts 
Conformed facts use standardized definitions of terms across individual marts. Different business users may use 
the same term in different ways. ‘Customer additions’ may be different from ‘gross additions’ or ‘adjusted 
additions.’ Developers need to be keenly aware of things that may be named the same but actually represent 
different concepts across organizations, or conversely things that are named differently but are actually the same 
concept across organizations. 
1.3.4.3 Object-Oriented (UML) 
The Unified Modeling Language (UML) is a graphical language for modeling software. The UML has a variety 
of notations of which one (the class model) concerns databases. The UML class model specifies classes (entity 
types) and their relationship types (Blaha, 2013). 
Student
Stdntno : integer
Strtdt: date
Prgm: text
ExpctGraddt: date
ActlGraddt: date
Class Name 
Attributes
Operations 
Figure 41 UML Class Model 
Figure 41 illustrates the characteristics of a UML Class Model: 
•
A Class diagram resembles an ER diagram except that the Operations or Methods section is not present
in ER.
•
In ER, the closest equivalent to Operations would be Stored Procedures.
•
Attribute types (e.g., Date, Minutes) are expressed in the implementable application code language and
not in the physical database implementable terminology.
•
Default values can be optionally shown in the notation.
•
Access to data is through the class’ exposed interface. Encapsulation or data hiding is based on a
‘localization effect’. A class and the instances that it maintains are exposed through Operations.
 

