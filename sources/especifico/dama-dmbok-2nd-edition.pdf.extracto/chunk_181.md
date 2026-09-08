# página 182 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

178 • DMBOK2 
service(s). Parallels are often drawn between the concept of cloud computing and the electricity grid: end users 
consume power without needing to understand the component devices or infrastructure required to provide the 
service. However, virtualization can be on-premises or off-premises. 
Cloud computing is a natural evolution of the widespread adoption of virtualization, service oriented 
architectures, and utility computing. Here are some methods for implementing databases on the cloud: 
•
Virtual machine image: Cloud platforms allow users to purchase virtual machine instances for a
limited time. It is possible to run a database on these virtual machines. Users can either upload their
own machine image with a database installed on it, or use ready-made machine images that already
include an optimized installation of a database.
•
Database-as-a-service (DaaS): Some cloud platforms offer options for using a database-as-a-service,
without physically launching a virtual machine instance for the database. In this configuration,
application owners do not have to install and maintain the database on their own. Instead, the database
service provider is responsible for installing and maintaining the database, and application owners pay
according to their usage.
•
Managed database hosting on the cloud: Here the database is not offered as a service; instead, the
cloud provider hosts the database and manages it on the application owner’s behalf.
DBAs, in coordination with network and system administrators, need to establish a systematic integrated project 
approach to include standardization, consolidation, virtualization, and automation of data backup and recovery 
functions, as well as security of these functions.  
•
Standardization/consolidation: Consolidation reduces the number of data storage locations an
organization has, including the number of data stores and processes within a data center. Based on
Data Governance policy, Data Architects and DBAs may develop the standard procedures that include
identifying mission critical data, duration of data retention, data encryption procedures, and data
replication policies.
•
Server virtualization: Virtualization technologies allow equipment, such as servers from multiple data
centers, to be replaced or consolidated. Virtualization lowers capital and operational expenses and
reduces energy consumption. Virtualization technologies are also used to create virtual desktops,
which can then be hosted in data centers and rented out on a subscription basis. Gartner views
virtualization as a catalyst for modernization (Bittman, 2009). Virtualization provides data storage
operations much more flexibility in provisioning storage at local or cloud environment.
•
Automation: Data automation involves automating tasks such as provisioning, configuration,
patching, release management, and compliance.
•
Security: The security of data on virtual systems needs to be integrated with existing security of
physical infrastructures (see Chapter 7).
 

