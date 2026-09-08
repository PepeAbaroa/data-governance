# página 285 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA INTEGRATION AND INTEROPERABILITY • 281 
The hubs provide consistent views of the data with limited performance impact on the source systems. Data 
hubs even minimize the number of systems and extracts that must access the data sources, thus minimizing the 
impact on the source system resources. Adding new systems to the portfolio only requires building interfaces to 
the data hub. Hub-and-spoke interaction is more efficient and can be cost-justified even if the number of 
systems involved is relatively small, but it becomes critical to managing a portfolio of systems in the hundreds 
or thousands.  
Enterprise Service Buses (ESB) are the data integration solution for near real-time sharing of data between 
many systems, where the hub is a virtual concept of the standard format or the canonical model for sharing data 
in the organization. 
Hub-and-spoke may not always be the best solution. Some hub-and-spoke model latency is unacceptable or 
performance is insufficient. The hub itself creates overhead in a hub-and-spoke architecture. A point-to-point 
solution would not require the hub. However, the benefits of the hub outweigh the drawbacks of the overhead as 
soon as three or more systems are involved in sharing data. Use of the hub-and-spoke design pattern for the 
interchange of data can drastically reduce the proliferation of data transformation and integration solutions and 
thus dramatically simplify the necessary organizational support.  
1.3.6.3 Publish - Subscribe 
A publish and subscribe model involves systems pushing data out (publish), and other systems pulling data in 
(subscribe). Systems providing data are listed in a catalog of data services, and systems looking to consume data 
subscribe to those services. When data is published, the data is automatically sent to the subscribers. 
When multiple data consumers want a certain set of data or data in a certain format, developing that data set 
centrally and making it available to all who need it ensures that all constituents receive a consistent data set in a 
timely manner. 
1.3.7 DII Architecture Concepts 
1.3.7.1 Application Coupling 
Coupling describes the degree to which two systems are entwined. Two systems that are tightly coupled usually 
have a synchronous interface, where one system waits for a response from the other. Tight coupling represents a 
riskier operation: if one system is unavailable then they are both effectively unavailable, and the business 
continuity plan for both have to be the same. (See Chapter 6.) 
Where possible, loose coupling is a preferred interface design, where data is passed between systems without 
waiting for a response and one system may be unavailable without causing the other to be unavailable. Loose 
 

