# página 206 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

202 • DMBOK2 
Most organizations also obtain some data from external third-party sources, such as lists of potential customers 
purchased from an information broker, postal and address information, or product data provided by a supplier. 
The data can be licensed or provided as an open data service, free of charge; provided in a number of different 
formats (CD, DVD, EDI, XML, RSS feeds, text files); or provided upon request or regularly updated via a 
subscription service. Some acquisitions require legal agreements. DBAs need to be aware of these restrictions 
before loading data.  
DBAs may be asked to handle these types of loads, or to create the initial load map. Limit manual execution of 
these loads to installations or other one-time situations, or ensure they are automated and scheduled. 
A managed approach to data acquisition centralizes responsibility for data subscription services with data 
analysts. The data analyst will need to document the external data source in the logical data model and data 
dictionary. A developer may design and create scripts or programs to read the data and load it into a database. 
The DBA will be responsible for implementing the necessary processes to load the data into the database and / 
or make it available to the application. 
2.2.3.6 Manage Data Replication  
DBAs can influence decisions about the data replication process by advising on: 
•
Active or passive replication
•
Distributed concurrency control from distributed data systems
•
The appropriate methods to identify updates to data through either timestamp or version numbers
under Change Data Control process
For small systems or data objects, complete data refreshes may satisfy the requirements for concurrency. For 
larger objects where most of the data does NOT change, merging changes into the data object is more efficient 
than completely copying all data for every change. For large objects where most of the data is changed, it may 
still be better to do a refresh than to incur the overhead of so many updates. 
2.2.4 Manage Database Performance 
The Database performance depends on two interdependent facets: availability and speed. Performance includes 
ensuring availability of space, query optimization, and other factors that enable a database to return data in an 
efficient way. Performance cannot be measured without availability. An unavailable database has a performance 
measure of zero. DBAs and NSAs manage database performance by: 
•
Setting and tuning operating system and application parameters.
•
Managing database connectivity. NSAs and DBAs provide technical guidance and support for IT and
business users requiring database connectivity based on policies enforced through standards and
protocols of the organization.
 

