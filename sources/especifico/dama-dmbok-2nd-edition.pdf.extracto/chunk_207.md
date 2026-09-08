# página 208 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

204 • DMBOK2 
2.2.4.2 Manage Database Availability 
Availability is the percentage of time that a system or database can be used for productive work. As 
organizations increase their uses of data, availability requirements increase, as do the risks and costs of 
unavailable data. To meet higher demand, maintenance windows are shrinking. Four related factors affect 
availability: 
•
Manageability: The ability to create and maintain an environment
•
Recoverability: The ability to reestablish service after interruption, and correct errors caused by
unforeseen events or component failures
•
Reliability: The ability to deliver service at specified levels for a stated period
•
Serviceability: The ability to identify the existence of problems, diagnose their causes, and repair /
solve them
Many things may prevent databases from being available, including: 
•
Planned outages
o
For maintenance
o
For upgrades
•
Unplanned outages
o
Loss of the server hardware
o
Disk hardware failure
o
Operating system failure
o
DBMS software failure
o
Data center site loss
o
Network failure
•
Application problems
o
Security and authorization problems
o
Severe performance problems
o
Recovery failures
•
Data problems
o
Corruption of data (due to bugs, poor design, or user error)
o
Loss of database objects
o
Loss of data
o
Data replication failure
•
Human error
DBAs are responsible for doing everything possible to ensure databases stay online and operational, including: 
•
Running database backup utilities
•
Running database reorganization utilities
•
Running statistics gathering utilities
•
Running integrity checking utilities
•
Automating the execution of these utilities
 

