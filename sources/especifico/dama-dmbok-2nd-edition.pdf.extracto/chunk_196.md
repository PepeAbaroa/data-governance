# página 197 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 193 
•
Critical recovery refers to a plan to restore the system as quickly as possible in order to minimize
delays or shut downs of business processes.
•
Non-critical recovery means that restoration of function can be delayed until systems that are more
critical have been restored.
Data processing errors include data load failures, query return failures, and obstacles to completing ETL or 
other processes. Common ways of increasing resilience in data processing systems are to trap and re-route data 
causing errors, detect and ignore data causing errors, and implement flags in processing for completed steps to 
avoid reprocessing data or repeating completed steps when restarting a process. 
Each system should require a certain level of resiliency (high or low). Some applications may require that any 
error halts all processing (low resiliency), while others may only require that the errors be trapped and re-routed 
for review, if not outright ignored. 
For extremely critical data, the DBA will need to implement a replication pattern in which data moves to 
another copy of the database on a remote server. In the event of database failure, applications can then ‘fail 
over’ to the remote database and continue processing.  
1.3.10.7 Retention 
Data Retention refers to how long data is kept available. Data retention planning should be part of the physical 
database design. Retention requirements also affect capacity planning.  
Data Security also affects data retention plans, as some data needs to be retained for specific timeframes for 
legal reasons. Failure to retain data for the appropriate length of time can have legal consequences. Likewise, 
there are also regulations related to purging data. Data can become a liability if kept longer than specified. 
Organizations should formulate retention policies based on regulatory requirements and risk management 
guidelines. These policies should drive specifications for purging and archiving of data.  
1.3.10.8 Sharding 
Sharding is a process where small chunks of the database are isolated and can be updated independently of other 
shards, so replication is merely a file copy. Because the shards are small, refreshes/overwrites may be optimal. 
2. Activities
The two main activities in Data Operations and Storage are Database Technology Support and Database 
Operations Support. Database Technology Support is specific to selecting and maintaining the software that 
 

