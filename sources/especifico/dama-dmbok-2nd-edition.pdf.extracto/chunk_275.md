# página 276 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

272 • DMBOK2 
The need to manage complexity and the costs associated with complexity are reasons to architect data 
integration from an enterprise perspective. An enterprise design of data integration is demonstrably more 
efficient and cost effective than distributed or point-to-point solutions. Developing point-to-point solutions 
between applications can result in thousands to millions of interfaces and can quickly overwhelm the 
capabilities of even the most effective and efficient IT support organization.  
Data hubs such as data warehouses and Master Data solutions help to alleviate this problem by consolidating 
the data needed by many applications and providing those applications with consistent views of the data. 
Similarly, the complexity of managing operational and transactional data that needs to be shared across the 
organization can be greatly simplified using enterprise data integration techniques such as hub-and-spoke 
integration and canonical message models.  
Another business driver is managing the cost of support. Moving data using multiple technologies, each 
requiring specific development and maintenance skills, can drive support costs up. Standard tool 
implementations can reduce support and staffing costs and improve the efficiency of troubleshooting efforts. 
Reducing the complexity of interface management can lower the cost of interface maintenance, and allow 
support resources to be more effectively deployed on other organizational priorities.  
DII also supports an organization’s ability to comply with data handling standards and regulations. Enterprise-
level DII systems enable re-use of code to implement compliance rules and simplify verification of compliance.  
1.2 Goals and Principles  
The implementation of Data Integration and Interoperability practices and solutions aims to: 
•
Make data available in the format and timeframe needed by data consumers, both human and system
•
Consolidate data physically and virtually into data hubs
•
Lower cost and complexity of managing solutions by developing shared models and interfaces
•
Identify meaningful events (opportunities and threats) and automatically trigger alerts and actions
•
Support Business Intelligence, analytics, Master Data Management, and operational efficiency efforts
When implementing DII, an organization should follow these principles: 
•
Take an enterprise perspective in design to ensure future extensibility, but implement through iterative
and incremental delivery
•
Balance local data needs with enterprise data needs, including support and maintenance.
•
Ensure business accountability for Data Integration and Interoperability design and activity. Business
experts should be involved in the design and modification of data transformation rules, both persistent
and virtual.
 

