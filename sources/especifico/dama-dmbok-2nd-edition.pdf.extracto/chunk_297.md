# página 298 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

294 • DMBOK2 
Data interaction capabilities must be monitored and serviced at the same service level as the most demanding 
target application or data consumer.  
3. Tools
3.1 Data Transformation Engine/ETL Tool 
A data transformation engine (or ETL tool) is the primary tool in the data integration toolbox, central to every 
enterprise data integration program. These tools usually support the operation as well as the design of the data 
transformation activities. 
Extremely sophisticated tools exist to develop and perform ETL, whether batch or real-time, physically or 
virtually. For single use point-to-point solutions, data integration processing is frequently implemented through 
custom coding. Enterprise level solutions usually require the use of tools to perform this processing in a 
standard way across the organization.  
Basic considerations in selecting a data transformation engine should include whether it is necessary to handle 
batch as well as real-time functionality, and whether unstructured as well as structured data needs to be 
accommodated, as the most mature tools exist for batch-oriented processing of structured data only. 
3.2 Data Virtualization Server 
Data transformation engines usually perform extract, transform, and load physically on data; however, data 
virtualization servers perform data extract, transform, and integrate virtually. Data virtualization servers can 
combine structured and unstructured data. A data warehouse is frequently an input to a data virtualization 
server, but a data virtualization server does not replace the data warehouse in the enterprise information 
architecture.  
3.3 Enterprise Service Bus 
An enterprise service bus (ESB) refers to both a software architecture model and a type of message-oriented 
middleware used to implement near real-time messaging between heterogeneous data stores, applications, and 
servers that reside within the same organization. Most internal data integration solutions that need to execute 
more frequent than daily use this architecture and this technology. Most commonly, an ESB is used in 
asynchronous format to enable the free flow of data. An ESB can also be used synchronously in certain 
situations. 
 

