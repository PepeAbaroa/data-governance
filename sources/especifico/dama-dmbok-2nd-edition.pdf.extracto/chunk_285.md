# página 286 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

282 • DMBOK2 
coupling can be implemented using various techniques with services, APIs, or message queues. Figure 69 
illustrates a possible loose coupling design. 
Figure 69 Application Coupling 
Service Oriented Architecture using an Enterprise Service Bus is an example of a loosely coupled data 
interaction design pattern. 
Where the systems are loosely coupled, replacement of systems in the application inventory can theoretically be 
performed without rewriting the systems with which they interact, because the interaction points are well-
defined. 
1.3.7.2 Orchestration and Process Controls 
Orchestration is the term used to describe how multiple processes are organized and executed in a system. All 
systems handling messages or data packets must be able to manage the order of execution of those processes, in 
order to preserve consistency and continuity. 
Process Controls are the components that ensure shipment, delivery, extraction, and loading of data is accurate 
and complete. An often-overlooked aspect of basic data movement architecture, controls include: 
•
Database activity logs
•
Batch job logs
•
Alerts
•
Exception logs
•
Job dependence charts with remediation options, standard responses
•
Job ‘clock’ information, such as the timing of dependent jobs, the expected length of the jobs, and the
computing (available) window time
Process A
Process B
Process A
Process B
Service
Tight Coupling
Loose Coupling
API
API
 

[6 imágenes en esta página]
