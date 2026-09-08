# página 185 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 181 
An interesting use of this theorem drives the Lambda Architecture design discussed in Chapter 14. Lambda 
Architecture uses two paths for data: a Speed path where availability and partition tolerance are most important, 
and a Batch path where consistency and availability are most important. 
1.3.6 Data Storage Media 
Data can be stored on a variety of media, including disks, volatile memory, and flash drives. Some systems can 
combine multiple storage types. The most commonly used are Disk and Storage Area Networks (SAN), In-
Memory, Columnar Compression Solutions, Virtual Storage Area Network VSAN, Cloud-based storage 
solutions, Radio Frequency Identification (RFID), Digital wallets, Data centers and Private, Public, and Hybrid 
Cloud Storage. (See Chapter 14.) 
1.3.6.1 Disk and Storage Area Networks (SAN) 
Disk storage is a very stable method of storing data persistently. Multiple types of disk can exist in the same 
system. Data can be stored according to usage patterns, with less-used data stored on slower-access disks, which 
are usually cheaper than high performance disk systems.  
Disk arrays can be collected into Storage Area Networks (SAN). Data movement on a SAN may not require a 
network, as data can be moved on the backplane. 
1.3.6.2 In-Memory 
In-Memory databases (IMDB) are loaded from permanent storage into volatile memory when the system is 
turned on, and all processing occurs within the memory array, providing faster response time than disk-based 
systems. Most in-memory databases also have features to set and configure durability in case of unexpected 
shutdown.  
If the application can be reasonably assured to fit most/all data into memory, then significant optimization can 
be made available from in-memory database systems. These IMDB’s provide more predictable access time to 
data than do disk storage mechanisms, but they require a much larger investment. IMDB’s provide functionality 
for real-time processing of analytics and are generally reserved for this due to the investment required.  
1.3.6.3 Columnar Compression Solutions 
Columnar-based databases are designed to handle data sets in which data values are repeated to a great extent. 
For example, in a table with 256 columns, a lookup for a value that exists in a row will retrieve all the data in 
the row (and be somewhat disk-bound). Columnar storage reduces this I/O bandwidth by storing column data 
 

