# página 281 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA INTEGRATION AND INTEROPERABILITY • 277 
In log-based change data captures, data activity logs created by the database management system are copied and 
processed, looking for specific changes that are then translated and applied to a target database. Complex 
translations may be difficult, but intermediary structures resembling the source object can be used as a way of 
staging the changes for further processing. 
1.3.2.3 Near-real-time and Event-driven 
Most data integration solutions that are not performed in batches use a near-real-time or event-driven solution. 
Data is processed in smaller sets spread across the day in a defined schedule, or data is processed when an event 
happens, such as a data update. Near-real-time processing has a lower latency than batch processing and often a 
lower system load as the work is distributed over time, but it is usually slower than a synchronized data 
integration solution. Near-real-time data integration solutions are usually implemented using an enterprise 
service bus. 
State information and process dependencies must be monitored by the target application load process. Data 
coming into the target may not be available in the exact order that the target needs to build the correct target 
data. For example, process Master Data or dimensional data prior to transactional data that uses that Master 
Data. 
1.3.2.4 Asynchronous 
In an asynchronous data flow, the system providing data does not wait for the receiving system to acknowledge 
update before continuing processing. Asynchronous implies that either the sending or receiving system could be 
off-line for some period without the other system also being off-line.  
Asynchronous data integration does not prevent the source application from continuing its processing, or cause 
the source application to be unavailable if any of the target applications are unavailable. Since the data updates 
made to applications in an asynchronous configuration are not immediate, the integration is called near-real-
time. The delay between updates made in the source and relayed to target data sets in a near-real-time 
environment is usually measured in seconds or minutes.  
1.3.2.5 Real-time, Synchronous 
There are situations where no time delay or other differences between source and target data is acceptable. 
When data in one data set must be kept perfectly in synch with the data in another data set, then a real-time, 
synchronous solution must be used.  
In a synchronous integration solution, an executing process waits to receive confirmation from other 
applications or processes prior to executing its next activity or transaction. This means that the solution can 
process fewer transactions because it has to spend time waiting for confirmation of data synchronization. If any 
 

