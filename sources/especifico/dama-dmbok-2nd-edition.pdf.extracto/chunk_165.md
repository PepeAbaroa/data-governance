# página 166 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

162 • DMBOK2 
•
Reusability: The database structure should ensure that, where appropriate, multiple applications can
use the data and that the data can serve multiple purposes (e.g., business analysis, quality
improvement, strategic planning, customer relationship management, and process improvement).
Avoid coupling a database, data structure, or data object to a single application.
•
Integrity: The data should always have a valid business meaning and value, regardless of context, and
should always reflect a valid state of the business. Enforce data integrity constraints as close to the data
as possible, and immediately detect and report violations of data integrity constraints.
•
Security: True and accurate data should always be immediately available to authorized users, but only
to authorized users. The privacy concerns of all stakeholders, including customers, business partners,
and government regulators, must be met. Enforce data security, like data integrity, as close to the data
as possible, and immediately detect and report security violations.
•
Maintainability: Perform all data work at a cost that yields value by ensuring that the cost of creating,
storing, maintaining, using, and disposing of data does not exceed its value to the organization. Ensure
the fastest possible response to changes in business processes and new business requirements.
5. Data Model Governance
5.1 Data Model and Design Quality Management 
Data analysts and designers act as intermediaries between information consumers (the people with business 
requirements for data) and the data producers who capture the data in usable form. Data professionals must 
balance the data requirements of the information consumers and the application requirements of data producers. 
Data professionals must also balance the short-term versus long-term business interests. Information consumers 
need data in a timely fashion to meet short-term business obligations and to take advantage of current business 
opportunities. System-development project teams must meet time and budget constraints. However, they must 
also meet the long-term interests of all stakeholders by ensuring that an organization’s data resides in data 
structures that are secure, recoverable, sharable, and reusable, and that this data is as correct, timely, relevant, 
and usable as possible. Therefore, data models and database designs should be a reasonable balance between the 
short-term needs and the long-term needs of the enterprise. 
5.1.1 Develop Data Modeling and Design Standards 
As previously noted (in Section 4.1) data modeling and database design standards provide guiding principles to 
meet business data requirements, conform to Enterprise and Data Architecture standards, and ensure the quality 
of data. Data modeling and database design standards should include the following: 
 

