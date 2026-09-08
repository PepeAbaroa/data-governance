# página 398 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

394 • DMBOK2 
1.3.8.3 Near-real-time and Real-time 
With the onset of Operational BI (or Operational Analytics) pushing for lower latency and more integration of 
real-time or near-real-time data into the data warehouse, new architectural approaches emerged to deal with the 
inclusion of volatile data. For example, a common application of operational BI is the automated banking 
machine data provisioning. When making a banking transaction, historical balances and new balances resulting 
from immediate banking actions need to be presented to the banking customer real-time. Two key design 
concepts that are required for provisioning data in near-real-time are isolation of change and alternatives to 
batch processing. 
The impact of the changes from new volatile data must be isolated from the bulk of the historical, non-volatile 
DW data. Typical architectural approaches for isolation include a combination of building partitions and using 
union queries for the different partitions. Alternatives to batch processing handle the increasingly shorter 
latency requirements for data availability in the DW. There are three main types: trickle feeds, messaging, and 
streaming, which differ by where data is accumulated while waiting to be processed. (See Chapter 8.) 
•
Trickle feeds (Source accumulation): Rather than run on a nightly schedule, trickle feeds execute
batch loads on a more frequent schedule (e.g., hourly, every 5 minutes) or when a threshold is reached
(e.g., 300 transactions, 1G of data). This allows some processing to happen during the day, but not as
intensely as with a dedicated nightly batch process. Care is needed to ensure that if a trickle feed batch
takes longer to complete than the time between feeds, the next feed is delayed so that the data is still
loaded in proper order.
•
Messaging (Bus accumulation): Message interaction in real-time or near-real-time is useful when
extremely small packets of data (messages, events, or transactions) are published to a bus as they
occur. Target systems subscribe to the bus, and incrementally process the packets into the warehouse
as needed. Source systems and target systems are independent of each other. Data-as-a-Service (DaaS)
frequently uses this method.
•
Streaming (Target accumulation): Rather than wait on a source-based schedule or threshold, a target
system collects data as it is received into a buffer area or queue, and processes it in order. The result
interaction or some aggregate may later appear as an additional feed to the warehouse.
2. Activities
2.1 Understand Requirements 
Developing a data warehouse is different from developing an operational system. Operational systems depend 
on precise, specific requirements. Data warehouses bring together data that will be used in a range of different 
ways. Moreover, usage will evolve over time as users analyze and explore data. Take time in the initial phases 
 

