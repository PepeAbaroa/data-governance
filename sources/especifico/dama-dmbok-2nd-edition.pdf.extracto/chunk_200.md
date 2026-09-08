# página 201 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 197 
•
Transaction-based
•
Large data set write- or retrieval-based
•
Time-based (heavier at month end, lighter on weekends, etc.),
•
Location-based (more densely populated areas have more transactions, etc.)
•
Priority-based (some departments or batch IDs have higher priority than others)
Some systems will have a combination of these basic patterns. DBAs need to be able to predict ebbs and flows 
of usage patterns and have processes in place to handle peaks (such as query governors or priority management) 
as well as to take advantage of valleys (delay processes that need large amounts of resources until a valley 
pattern exists). This information can be used to maintain database performance.  
2.2.1.3 Define Access Requirements 
Data access includes activities related to storing, retrieving, or acting on data housed in a database or other 
repository. Data Access is simply the authorization to access different data files.  
Various standard languages, methods, and formats exist for accessing data from databases and other 
repositories: SQL, ODBC, JDBC, XQJ, ADO.NET, XML, X Query, X Path, and Web Services for ACID-type 
systems. BASE-type access method standards include C, C++, REST, XML, and Java36. Some standards enable 
translation of data from unstructured (such as HTML or free-text files) to structured (such as XML or SOL).  
Data architects and DBAs can assist organizations to select appropriate methods and tools required for data 
access. 
2.2.2 Plan for Business Continuity 
Organizations need to plan for business continuity in the event of disaster or adverse event that impacts their 
systems and their ability to use their data. DBAs must make sure a recovery plan exists for all databases and 
database servers, covering scenarios that could result in loss or corruption of data, such as: 
•
Loss of the physical database server
•
Loss of one or more disk storage devices
•
Loss of a database, including the DBMS Master Database, temporary storage database, transaction log
segment, etc.
•
Corruption of database index or data pages
•
Loss of the database or log segment filesystems
•
Loss of database or transaction log backup files
36  http://bit.ly/1rWAUxS (accessed 2/28/2016) has a list of all data access methods for BASE-type systems. 
 

