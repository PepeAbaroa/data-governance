# página 204 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

200 • DMBOK2 
•
During the configuration identification process, DBAs will work with data stewards, data architects,
and data modelers to identify the attributes that define every aspect of a configuration for end-user
purposes. These attributes are recorded in configuration documentation and baselined. Once an
attribute is baselined a formal configuration change control processes is required to change the
attribute.
•
Configuration change control is a set of processes and approval stages required to change a
configuration item’s attributes and to re-baseline them.
•
Configuration status accounting is the ability to record and report on the configuration baseline
associated with each configuration item at any point in time.
•
Configuration audits occur both at delivery and when effecting a change. There are two types. A
physical configuration audit ensures that a configuration item is installed in accordance with the
requirements of its detailed design documentation, while a functional configuration audit ensures that
performance attributes of a configuration item are achieved.
To maintain data integrity and traceability throughout the data lifecycle, DBAs communicate the changes to 
physical database attributes to modelers, developers, and Metadata managers.  
DBAs must also maintain metrics on data volume, capacity projections, and query performance, as well as 
statistics on physical objects, in order to identify data replication needs, data migration volumes, and data 
recovery checkpoints. Larger databases will also have object partitioning, which must be monitored and 
maintained over time to ensure that the object maintains the desired distribution of data. 
2.2.3.2 Manage Database Access Controls 
DBAs are responsible for managing the controls that enable access to the data. DBAs oversee the following 
functions to protect data assets and data integrity: 
•
Controlled environment: DBAs work with NSAs to manage a controlled environment for data assets;
this includes network roles and permissions management, 24x7 monitoring and network health
monitoring, firewall management, patch management, and Microsoft Baseline Security Analyzer
(MBSA) integration.
•
Physical security: The physical security of data assets is managed by Simple Network Management
Protocol (SNMP)-based monitoring, data audit logging, disaster management, and database backup
planning. DBAs configure and monitor these protocols. Monitoring is especially important for security
protocols.
•
Monitoring: Database systems are made available by continuous hardware and software monitoring of
critical servers.
 

