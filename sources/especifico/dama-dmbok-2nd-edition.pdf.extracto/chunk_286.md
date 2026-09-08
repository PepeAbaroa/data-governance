# página 287 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA INTEGRATION AND INTEROPERABILITY • 283 
1.3.7.3 Enterprise Application Integration (EAI) 
In an enterprise application integration model (EAI), software modules interact with one another only through 
well-defined interface calls (application programming interfaces – APIs). Data stores are updated only by their 
own software modules and other software cannot reach in to the data in an application but only access through 
the defined APIs. EAI is built on object-oriented concepts, which emphasize reuse and the ability to replace any 
module without impact on any other.  
1.3.7.4 Enterprise Service Bus (ESB) 
An Enterprise Service Bus is a system that acts as an intermediary between systems, passing messages between 
them. Applications can send and receive messages or files using the ESB, and are encapsulated from other 
processes existing on the ESB. An example of loose coupling, the ESB acts as the service between the 
applications. (See Figure 70.) 
Figure 70 Enterprise Service Bus 
1.3.7.5 Service-Oriented Architecture (SOA) 
Most mature enterprise data integration strategies utilize the idea of service-oriented architecture (SOA), where 
the functionality of providing data or updating data (or other data services) can be provided through well-
defined service calls between applications. With this approach, applications do not have to have direct 
interaction with or knowledge of the inner workings of other applications. SOA enables application 
independence and the ability for an organization to replace systems without needing to make significant 
changes to the systems that interfaced with them. 
Application n
Service n
Service 1
Application 1
Application 2
Process
Orchestration 
Manager
Enterprise Service Bus
 

[15 imágenes en esta página]
