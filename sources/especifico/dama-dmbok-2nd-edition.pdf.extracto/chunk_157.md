# página 158 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

154 • DMBOK2 
•
Select Scheme: Decide whether the data model should be built following a relational, dimensional,
fact-based, or NoSQL scheme. Refer to the earlier discussion on scheme and when to choose each
scheme (see Section 1.3.4).
•
Select Notation: Once the scheme is selected, choose the appropriate notation, such as information
engineering or object role modeling. Choosing a notation depends on standards within an organization
and the familiarity of users of a particular model with a particular notation.
•
Complete Initial CDM: The initial CDM should capture the viewpoint of a user group. It should not
complicate the process by trying to figure out how their viewpoint fits with other departments or with
the organization as a whole.
o
Collect the highest-level concepts (nouns) that exist for the organization. Common concepts
are Time, Geography, Customer/Member/Client, Product/Service, and Transaction.
o
Then collect the activities (verbs) that connect these concepts. Relationships can go both
ways, or involve more than two concepts. Examples are: Customers have multiple
Geographic Locations (home, work, etc.), Geographic Locations have many Customers.
Transactions occur at a Time, at a Facility, for a Customer, selling a Product.
•
Incorporate Enterprise Terminology: Once the data modeler has captured the users’ view in the
boxes and lines, the data modeler next captures the enterprise perspective by ensuring consistency with
enterprise terminology and rules. For example, there would be some reconciliation work involved if
the audience conceptual data model had an entity called Client, and the enterprise perspective called
this same concept Customer.
•
Obtain Sign-off: After the initial model is complete, make sure the model is reviewed for data
modeling best practices as well as its ability to meet the requirements. Usually email verification that
the model looks accurate will suffice.
2.2.1.2 Logical Data Modeling 
A logical data model (LDM) captures the detailed data requirements within the scope of a CDM. 
2.2.1.2.1 Analyze Information Requirements 
To identify information requirements, one must first identify business information needs, in the context of one 
or more business processes. As their input, business processes require information products that are themselves 
the output from other business processes. The names of these information products often identify an essential 
business vocabulary that serves as the basis for data modeling. Regardless of whether processes or data are 
modeled sequentially (in either order), or concurrently, effective analysis and design should ensure a relatively 
balanced view of data (nouns) and processes (verbs), with equal emphasis on both process and data modeling. 
 

