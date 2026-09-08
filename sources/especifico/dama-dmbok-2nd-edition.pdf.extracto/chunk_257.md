# página 258 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

254 • DMBOK2 
Metadata. It can be implemented within a system or across dependent heterogeneous systems. It can focus on 
specific privileges, such as the ability to download large sets of data or to access data at off hours.  
Monitoring can be automated or executed manually or executed through a combination of automation and 
oversight. Automated monitoring does impose overhead on the underlying systems and may affect system 
performance. Periodic snapshots of activity can be useful in understanding trends and comparing against 
standards criteria. Iterative configuration changes may be required to achieve the optimal parameters for proper 
monitoring. 
Automated recording of sensitive or unusual database transactions should be part of any database deployment. 
Lack of automated monitoring represents serious risks:  
•
Regulatory risk: Organizations with weak database audit mechanisms will increasingly find that they
are at odds with government regulatory requirements. Sarbanes-Oxley (SOX) in the financial services
sector and the Healthcare Information Portability and Accountability Act (HIPAA) in the healthcare
sector are just two examples of US government regulation with clear database audit requirements.
•
Detection and recovery risk: Audit mechanisms represent the last line of defense. If an attacker
circumvents other defenses, audit data can identify the existence of a violation after the fact. Audit data
can also be used to link a violation to a particular user or as a guide to repair the system.
•
Administrative and audit duties risk: Users with administrative access to the database server –
whether that access was obtained legitimately or maliciously – can turn off auditing to hide fraudulent
activity. Audit duties should ideally be separate from both database administrators and the database
server platform support staff.
•
Risk of reliance on inadequate native audit tools: Database software platforms often try to integrate
basic audit capabilities but they often suffer from multiple weaknesses that limit or preclude
deployment. When users access the database via Web applications (such as SAP, Oracle E-Business
Suite, or PeopleSoft), native audit mechanisms have no awareness of specific user identities and all
user activity is associated with the Web application account name. Therefore, when native audit logs
reveal fraudulent database transactions, there is no link to the responsible user.
To mitigate the risks, implement a network-based audit appliance, which can address most of the weaknesses 
associated with native audit tools, but which does not take place of regular audits by trained auditors. This kind 
of appliance has the following benefits:  
•
High performance: Network-based audit appliances can operate at line speed with little impact on
database performance.
•
Separation of duties: Network-based audit appliances should operate independently of database
administrators making it possible to separate audit duties from administrative duties as appropriate.
 

