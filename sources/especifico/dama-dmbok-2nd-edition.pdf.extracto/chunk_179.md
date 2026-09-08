# página 180 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

176 • DMBOK2 
management software is also designed to detect and handle failures. While any given computer may fail, the 
system overall is unlikely to.  
Some distributed databases implement a computational paradigm named MapReduce to further improve 
performance. In MapReduce, the data request is divided into many small fragments of work, each of which may 
be executed or re-executed on any node in the cluster. In addition, data is co-located on the compute nodes, 
providing very high aggregate bandwidth across the cluster. Both the filesystem and the application are 
designed to automatically handle node failures. 
1.3.4.2.1 Federated Databases 
Federation provisions data without additional persistence or duplication of source data. A federated database 
system maps multiple autonomous database systems into a single federated database. The constituent databases, 
sometimes geographically separated, are interconnected via a computer network. They remain autonomous yet 
participate in a federation to allow partial and controlled sharing of their data. Federation provides an alternative 
to merging disparate databases. There is no actual data integration in the constituent databases because of data 
federation; instead, data interoperability manages the view of the federated databases as one large object (see 
Chapter 8). In contrast, a non-federated database system is an integration of component DBMS’s that are not 
autonomous; they are controlled, managed and governed by a centralized DBMS.  
Federated databases are best for heterogeneous and distributed integration projects such as enterprise 
information integration, data virtualization, schema matching, and Master Data Management. 
Federated architectures differ based on levels of integration with the component database systems and the extent 
of services offered by the federation. A FDBMS can be categorized as either loosely or tightly coupled. 
Figure 56 Federated Databases 
Federated
User View
Location A
Location B
Location C
map
map
map
 

[3 imágenes en esta página]
