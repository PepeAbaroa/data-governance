# página 175 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 171 
1.1 Business Drivers 
Companies rely on their information systems to run their operations. Data Storage and Operations activities are 
crucial to organizations that rely on data. Business continuity is the primary driver of these activities. If a 
system becomes unavailable, company operations may be impaired or stopped completely. A reliable data 
storage infrastructure for IT operations minimizes the risk of disruption. 
1.2 Goals and Principles  
The goals of data storage and operations include: 
•
Managing the availability of data throughout the data lifecycle
•
Ensuring the integrity of data assets
•
Managing the performance of data transactions
Data Storage and Operations represent a highly technical side of data management. DBAs and others involved 
in this work can do their jobs better and help the overall work of data management when they follow these 
guiding principles:  
•
Identify and act on automation opportunities: Automate database development processes,
developing tools, and processes that shorten each development cycle, reduce errors and rework, and
minimize the impact on the development team. In this way, DBAs can adapt to more iterative (agile)
approaches to application development. This improvement work should be done in collaboration with
data modeling and Data Architecture.
•
Build with reuse in mind: Develop and promote the use of abstracted and reusable data objects that
prevent applications from being tightly coupled to database schemas (the so-called ‘object-relational
impedance mismatch’). A number of mechanisms exist to this end, including database views, triggers,
functions and stored procedures, application data objects and data-access layers, XML and XSLT,
ADO.NET typed data sets, and web services. The DBA should be able to assess the best approach
virtualizing data. The end goal is to make using the database as quick, easy, and painless as possible.
•
Understand and appropriately apply best practices: DBAs should promote database standards and
best practices as requirements, but be flexible enough to deviate from them if given acceptable reasons
for these deviations. Database standards should never be a threat to the success of a project.
•
Connect database standards to support requirements: For example, the Service Level Agreement
(SLA) can reflect DBA-recommended and developer-accepted methods of ensuring data integrity and
data security. The SLA should reflect the transfer of responsibility from the DBAs to the development
team if the development team will be coding their own database update procedures or data access
layer. This prevents an ‘all or nothing’ approach to standards.
 

