# página 283 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA INTEGRATION AND INTEROPERABILITY • 279 
Such a solution must synchronize the physically distributed data set copies. Most database management systems 
have replication utilities to do this work. These utilities work best when the data sets are all maintained in the 
same database management system technology. Replication solutions usually monitor the log of changes to the 
data set, not the data set itself. They minimize the impact on any operational applications because they do not 
compete with the applications for access to the data set. Only data from the change log passes between 
replicated copies. Standard replication solutions are near-real-time; there is a small delay between a change in 
one copy of the data set and another.  
Because the benefits of replication solutions — minimal effect on the source data set and minimal amount of 
data being passed — are very desirable, replication is used in many data integration solutions, even those that 
do not include long distance physical distribution. The database management utilities do not require extensive 
programming, so there tend to be few programming bugs.  
Replication utilities work optimally when source and target data sets are exact copies of each other. Differences 
between source and target introduce risks to synchronization. If the ultimate target is not an exact copy of the 
source then it is necessary to maintain a staging area to house an exact copy of the sources. This requires extra 
disk usage and possibly extra database technology.  
Data replication solutions are not optimal if changes to the data may occur at multiple copy sites. If it is possible 
that the same piece of data is changed at two different sites, then there is a risk that the data might get 
unsynchronized, or one of the sites may have their changes overwritten without warning. (See Chapter 6.) 
1.3.4 Archiving 
Data that is used infrequently or not actively used may be moved to an alternate data structure or storage 
solution that is less costly to the organization. ETL functions can be used to transport and possibly transform the 
archive data to the data structures in the archive environment. Use archives to store data from applications that 
are being retired, as well as data from production operational systems that have not been used for a long time, to 
improve operational efficiency.  
It is critical to monitor archive technology to ensure that the data is still accessible when technology changes. 
Having an archive in an older structure or format unreadable by newer technology can be a risk, especially for 
data that is still legally required. (See Chapter 9.) 
1.3.5 Enterprise Message Format / Canonical Model 
A canonical data model is a common model used by an organization or data exchange group that standardizes 
the format in which data will be shared. In a hub-and-spoke data interaction design pattern, all systems that 
want to provide or receive data interact only with a central information hub. Data is transformed from or to a 
sending or receiving system based on a common or enterprise message format for the organization (a canonical 
model). (See Chapter 5.) Use of a canonical model limits the number of data transformations needed by any 
 

