# página 196 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

192 • DMBOK2 
Replication transparency occurs when data is replicated between database servers so that the information 
remains consistent throughout the database system and users cannot tell or even know which database copy they 
are using.  
The two primary replication patterns are mirroring and log shipping (see Figure 60). 
•
In mirroring, updates to the primary database are replicated immediately (relatively speaking) to the
secondary database, as part of a two-phase commit process.
•
In log shipping, a secondary server receives and applies copies of the primary database’s transaction
logs at regular intervals.
The choice of replication method depends on how critical the data is, and how important it is that failover to the 
secondary server be immediate. Mirroring is usually a more expensive option than log shipping. For one 
secondary server, mirroring is effective; log shipping may be used to update additional secondary servers. 
Figure 60 Log Shipping vs. Mirroring 
1.3.10.6 Resiliency and Recovery 
Resiliency in databases is the measurement of how tolerant a system is to error conditions. If a system can 
tolerate a high level of processing errors and still function as expected, it is highly resilient. If an application 
crashes upon the first unexpected condition, that system is not resilient. If the database can detect and either 
abort or automatically recover from common processing errors (runaway query, for example), it is considered 
resilient. There are always some conditions that no system can detect in advance, such as a power failure, and 
those conditions are considered disasters.  
Three recovery types provide guidelines for how quickly recovery takes place and what it focuses on: 
•
Immediate recovery from some issues sometimes can be resolved through design; for example,
predicting and automatically resolving issues, such as those that might be caused by a failover to
backup system.
Log
Log
Log Shipping
Mirroring
Location A
Location A
Location B
Location B
data
data
data
create
synch
apply
 

[6 imágenes en esta página]
