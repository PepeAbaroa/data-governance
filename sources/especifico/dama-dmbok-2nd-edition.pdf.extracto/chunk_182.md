# página 183 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 179 
1.3.5 Database Processing Types 
There are two basic types of database processing. ACID and BASE are on opposite ends of a spectrum, so the 
coincidental names matching ends of a pH spectrum are helpful. The CAP Theorem is used to define how 
closely a distributed system may match either ACID or BASE. 
1.3.5.1 ACID 
The acronym ACID was coined in the early 1980’s as the indispensable constraint for achieving reliability 
within database transactions. For decades, it has provided transaction processing with a reliable foundation on 
which to build.34 
•
Atomicity: All operations are performed, or none of them is, so that if one part of the transaction fails,
then the entire transaction fails.
•
Consistency: The transaction must meet all rules defined by the system at all times and must void half-
completed transactions.
•
Isolation: Each transaction is independent unto itself.
•
Durability: Once complete, the transaction cannot be undone.
Relational ACID technologies are the dominant tools in relational database storage; most use SQL as the 
interface.  
1.3.5.2 BASE 
The unprecedented increase in data volumes and variability, the need to document and store unstructured data, 
the need for read-optimized data workloads, and subsequent need for greater flexibility in scaling, design, 
processing, cost, and disaster recovery gave rise to the diametric opposite of ACID, appropriately termed 
BASE: 
•
Basically Available: The system guarantees some level of availability to the data even when there are
node failures. The data may be stale, but the system will still give and accept responses.
•
Soft State: The data is in a constant state of flux; while a response may be given, the data is not
guaranteed to be current.
•
Eventual Consistency: The data will eventually be consistent through all nodes and in all databases,
but not every transaction will be consistent at every moment.
34 Jim Gray established the concept. Haerder and Rueter (1983) coined the term ACID. 
 

