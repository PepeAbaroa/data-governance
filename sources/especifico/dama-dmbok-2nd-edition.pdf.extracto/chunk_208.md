# página 209 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 205 
•
Exploiting table space clustering and partitioning
•
Replicating data across mirror databases to ensure high availability
2.2.4.3 Manage Database Execution 
DBAs also establish and monitor database execution, use of data change logs, and synchronization of duplicated 
environments. Log sizes and locations require space and in some cases can be treated like file-based databases 
on their own. Other applications that consume logs must also be managed, to ensure use of the correct logs at 
the required logging level. The more detail that is logged, the more space and processing required, which may 
adversely affect performance. 
2.2.4.4 Maintain Database Performance Service Levels 
DBAs optimize database performance both proactively and reactively, by monitoring performance and by 
responding to problems quickly and competently. Most DBMSs provide the capability of monitoring 
performance, allowing DBAs to generate analysis reports. Most server operating systems have similar 
monitoring and reporting capabilities. DBAs should run activity and performance reports against both the 
DBMS and the server on a regular basis, including during periods of heavy activity. They should compare these 
reports to previous reports to identify any negative trends and save them to help analyze problems over time. 
2.2.4.4.1 Transaction Performance vs. Batch Performance 
Data movement may occur in real time through online transactions. However, many data movement and 
transformation activities are performed through batch programs, which may move data between systems, or 
merely perform operations on data within a system. These batch jobs must complete within specified windows 
in the operating schedule. DBAs and data integration specialists monitor the performance of batch data jobs, 
noting exceptional completion times and errors, determining the root cause of errors, and resolving these issues. 
2.2.4.4.2 Issue Remediation 
When performance problems occur, the DBA, NSA, and Server Administration teams should use the 
monitoring and administration tools of the DBMS to help identify the source of the problem. Common reasons 
for poor database performance include: 
•
Memory allocation or contention: A buffer or cache for data.
•
Locking and blocking: In some cases, a process running in the database may lock up database
resources, such as tables or data pages, and block another process that needs them. If the problem
persists, the DBA can kill the blocking process. In some cases, two processes may ‘deadlock’, with
 

