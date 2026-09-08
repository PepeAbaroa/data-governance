# página 195 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 191 
way to replicate data changes to a target without affecting the source. In a simplified CDC context, one 
computer system has data that may have changed from a previous point in time, and a second computer system 
needs to reflect the same change. Rather than sending the entire database over the network to reflect just a few 
minor changes, the idea is to just send what changed (deltas), so that the receiving system can make appropriate 
updates. 
There are two different methods to detect and collect changes: data versioning, which evaluates columns that 
identify rows that have changed (e.g., last-update-timestamp columns, version-number columns, status-indicator 
columns), or by reading logs that document the changes and enable them to be replicated in secondary systems.  
1.3.10.4 Purging 
It is incorrect to assume that all data will reside forever in primary storage. Eventually, the data will fill the 
available space, and performance will begin to degrade. At that point, data will need to be archived, purged, or 
both. Just as importantly, some data will degrade in value and is not worth keeping. Purging is the process of 
completely removing data from storage media such that it cannot be recovered. A principal goal of data 
management is that the cost of maintaining data should not exceed its value to the organization. Purging data 
reduces costs and risks. Data to be purged is generally deemed obsolete and unnecessary, even for regulatory 
purposes. Some data may become a liability if kept longer than necessary. Purging it reduces the risks that it 
may be misused.  
1.3.10.5 Replication 
Data replication means same data is stored on multiple storage devices. In some situations, having duplicate 
databases is useful, such as in a high-availability environment where spreading the workload among identical 
databases in different hardware or even data centers can preserve functionality during peak usage times or 
disasters. 
Replication can be active or passive: 
•
Active replication is performed by recreating and storing the same data at every replica from every
other replica.
•
Passive replication involves recreating and storing data on a single primary replica and then
transforming its resultant state to other secondary replicas.
Replication has two dimensions of scaling: 
•
Horizontal data scaling has more data replicas.
•
Vertical data scaling has data replicas located further away in distance geographically.
Multi-master replication, where updates can be submitted to any database node and then ripple through to other 
servers, is often desired, but increases complexity and cost.  
 

