# página 523 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

BIG DATA AND DATA SCIENCE • 519 
Figure 102 Columnar Appliance Architecture95 
Data volumes are growing fast. Companies can grow the capacity and performance of their systems over time 
by adding new nodes. MPP makes it easy to expand the parallelism of hundreds or thousands of cores across an 
ever-growing pool of machines. A massively parallel, shared-nothing architecture fully uses each core, with 
linear scalability and increased processing performance on large data sets. 
3.2 Distributed File-based Databases 
Distributed file-based solutions technologies, such as the open source Hadoop, are an inexpensive way to store 
large amounts of data in different formats. Hadoop stores files of any type – structured, semi-structured, and 
unstructured. Using a configuration similar to MPP Shared-nothing (an MPP foundation for file storage), it 
shares files across processing servers. It is ideal for storing data securely (as many copies are made), but has 
challenges when trying to allow access to data via structured or analytical mechanism (like SQL).  
Due to its relatively low cost, Hadoop has become the landing zone of choice for many organizations. From 
Hadoop, data can be moved to MPP Shared-nothing databases to have algorithms run against it. Some 
organizations run complex Data Science queries in Hadoop, and are not concerned with response times in the 
order of hours and days (rather than minutes for the former architecture). 
The language used in file-based solutions is called MapReduce. This language has three main steps: 
•
Map: Identify and obtain the data to be analyzed
•
Shuffle: Combine the data according to the analytical patterns desired
95 Image Source: “Greenplum Database 4.0: Critical Mass Innovation”, White Paper, August 2010. 
SQL 
MapReduce
Master 
Servers
Interconnect 
Bus
Segment 
Servers
External 
Sources
 

[14 imágenes en esta página]
