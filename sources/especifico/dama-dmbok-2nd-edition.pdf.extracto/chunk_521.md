# página 522 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

518 • DMBOK2 
Access to unstructured data used to occur largely through a batch query interface that resulted in slow scheduled 
execution and poor response times. Several NoSQL databases are now available with designs that address 
specific limitations in this acquisition process. Scalable distributed databases automatically provide sharding 
capabilities (the ability to scale across servers natively) for parallel query execution. Of course, as with any 
other database, structural definition and mapping to unstructured data sets remain largely manual processes.  
Immediate query, reporting, and analysis capabilities can be satisfied with Big Data in-memory technologies 
that allow end users to construct SQL-like queries to access unstructured data. There are also adaptors to SQL 
for some tools that will transmit a NoSQL process and return a SQL compliant query – with limitations and 
caveats. Adaptor technologies can allow existing tools to be used for unstructured data query. 
Decision criteria tool sets, process implementation tools, and professional services offerings can both facilitate 
and expedite the process of choosing an initial set of tools. As when acquiring BI tools, it is critical to evaluate 
all options: build, buy, or rent (provisioned as software-as-a-service). As noted in Chapter 11, cloud sourcing 
tools and the associated expertise should be weighed against the cost of building from scratch or deploying 
purchased products from vendors. Ongoing upgrade and potential replacement costs must be considered as well. 
Alignment to a set OLA can bridge forecasted costs and provide input into setting compelling fees and penalties 
for term violations.  
3.1 MPP Shared-nothing Technologies and Architecture 
Massively Parallel Processing (MPP) Shared-nothing Database technologies have become the standard platform 
for Data Science-oriented analysis of Big Data sets. In MPP databases, data is partitioned (logically distributed) 
across multiple processing servers (computational nodes), with each server having its own dedicated memory to 
process data locally. Communication between processing servers is usually controlled by a master host and 
occurs over a network interconnect. There is no disk sharing or memory contention, hence the name, ‘shared-
nothing’. 
MPP has evolved because traditional computing paradigms (indexes, distributed data sets, etc.) did not provide 
acceptable response times on massive tables. Even the most powerful of computing platforms (Cray computer) 
would take many hours or even days to compute a complex algorithm against a trillion-row table. 
Consider now a number of commodity hardware servers, all lined up in a row and controlled via a host. Each is 
sent part of the query to run against this segmented or distributed trillion-row table. If there are, for example, 
1000 processing servers, the query changes from accessing a trillion rows in one table to accessing 1000 billion-
row tables. This type of computing architecture is linearly scalable, which adds to the appeal for data scientist 
and Big Data users requiring a scalable platform to incorporate growth. 
This technology also enabled in-database analytical functions – the ability to execute analytical functions (like 
K-means Clustering, Regression, etc.) at the processor level. Distribution of workload to the processor level 
greatly speeds up analytical queries – thereby fueling innovation in Data Science. 
A system that automatically distributes data and parallelizes query workloads across all available (localized) 
hardware is the optimum solution for Big Data analytics. 
 

