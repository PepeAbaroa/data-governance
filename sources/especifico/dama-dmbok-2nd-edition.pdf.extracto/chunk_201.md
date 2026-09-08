# página 202 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

198 • DMBOK2 
Each database should be evaluated for criticality so that its restoration can be prioritized. Some databases will 
be essential to business operations and will need to be restored immediately. Less critical databases will not be 
restored until primary systems are up and running. Still other may not need to be restored at all; for example, if 
they are merely copies that are refreshed when loaded. 
Management and the organization’s business continuity group, if one exists, should review and approve the data 
recovery plan. The DBA group should regularly review the plans for accuracy and comprehensiveness. Keep a 
copy of the plan, along with all the software needed to install and configure the DBMS, instructions, and 
security codes (e.g., the administrator password) in a secure, off-site location in the event of a disaster.  
No system can be recovered from a disaster if the backups are unavailable or unreadable. Regular backups are 
essential to any recovery effort, but if they are unreadable, they are worse than useless; processing time making 
the unreadable backups will have been wasted, along with the opportunity for fixing the issue that made the 
backups unreadable. Keep all backups in a secure, off-site location. 
2.2.2.1 Make Backups 
Make backups of databases and, if appropriate, the database transaction logs. The system’s Service Level 
Agreement (SLA) should specify backup frequency. Balance the importance of the data against the cost of 
protecting it. For large databases, frequent backups can consume large amounts of disk storage and server 
resources. In addition to incremental backups, periodically make a complete backup of each database. 
Furthermore, databases should reside on a managed storage area, ideally a RAID array on a storage area 
network or SAN, with daily back up to separate storage media. For OLTP databases, the frequency of 
transaction log backups will depend on the frequency of updating, and the amount of data involved. For 
frequently updated databases, more frequent log dumps will not only provide greater protection, but will also 
reduce the impact of the backups on server resources and applications.  
Backup files should be kept on a separate filesystem from the databases, and should be backed up to some 
separate storage medium as specified in the SLA. Store copies of the daily backups in a secure off-site facility. 
Most DBMSs support hot backups of the database – backups taken while applications are running. When some 
updates occur in transit, they will roll either forward to completion, or roll back when the backup reloads. The 
alternative is a cold backup taken when the database is off-line. However, a cold backup may not be a viable 
option if applications need to be continuously available. 
2.2.2.2 Recover Data 
Most backup software includes the option to read from the backup into the system. The DBA works with the 
infrastructure team to re-mount the media containing the backup and to execute the restoration. The specific 
utilities used to execute the restoration of the data depend on the type of databased.  
 

