# página 179 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 175 
1.3.3.4 NSA 
Network Storage Administrators are concerned with the hardware and software supporting data storage arrays. 
Multiple network storage array systems have different needs and monitoring requirements than simple database 
systems. 
1.3.4 Database Architecture Types 
A database can be classified as either centralized or distributed. A centralized system manages a single 
database, while a distributed system manages multiple databases on multiple systems. A distributed system’s 
components can be classified depending on the autonomy of the component systems into two types: federated 
(autonomous) or non-federated (non-autonomous). Figure 55 illustrates the difference between centralized and 
distributed. 
Figure 55 Centralized vs. Distributed 
1.3.4.1 Centralized Databases 
Centralized databases have all the data in one system in one place. All users come to the one system to access 
the data. For certain restricted data, centralization can be ideal, but for data that needs to be widely available, 
centralized databases have risks. For example, if the centralized system is unavailable, there are no other 
alternatives for accessing the data. 
1.3.4.2 Distributed Databases 
Distributed databases make possible quick access to data over a large number of nodes. Popular distributed 
database technologies are based on using commodity hardware servers. They are designed to scale out from 
single servers to thousands of machines, each offering local computation and storage. Rather than rely on 
hardware to deliver high-availability, the database management software itself is designed to replicate data 
amongst the servers, thereby delivering a highly available service on top of a cluster of computers. Database 
Centralized
Distributed, not Federated
User View
User View
Location A
Location A
Location B
Location C
 

[3 imágenes en esta página]
