# página 279 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA INTEGRATION AND INTEROPERABILITY • 275 
transformations to occur after the load to the target system, often as part of the process. ELT allows source data 
to be instantiated on the target system as raw data, which can be useful for other processes. This is common in 
Big Data environments where ELT loads the data lake. (See Chapter 14.) 
Figure 68 ELT Process Flow 
1.3.1.5 Mapping 
A synonym for transformation, a mapping is both the process of developing the lookup matrix from source to 
target structures and the result of that process. A mapping defines the sources to be extracted, the rules for 
identifying data for extraction, targets to be loaded, rules for identifying target rows for update (if any), and any 
transformation rules or calculations to be applied. Many data integration tools offer visualizations of mappings 
that enable developers to use graphical interfaces to create transformation code. 
1.3.2 Latency 
Latency is the time difference between when data is generated in the source system and when the data is 
available for use in the target system. Different approaches to data processing result in different degrees of data 
latency. Latency can be high (batch) or low (event-driven) to very low (real-time synchronous). 
1.3.2.1 Batch 
Most data moves between applications and organizations in clumps or files either on request by a human data 
consumer or automatically on a periodic schedule. This type of interaction is called batch or ETL.  
Lookups
Mappings
Extract
Process
Load
Process
Transform
Process
Source
Datastore
Target
Datastore
 

[8 imágenes en esta página]
