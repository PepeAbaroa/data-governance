# página 509 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

BIG DATA AND DATA SCIENCE • 505 
1.3.6 Data Lake 
A data lake is an environment where a vast amount of data of various types and structures can be ingested, 
stored, assessed, and analyzed. Data lakes can serve many purposes. For example, providing 
•
An environment for Data Scientists to mine and analyze data
•
A central storage area for raw data, with minimal, if any, transformation
•
Alternate storage for detailed historical data warehouse data
•
An online archive for records
•
An environment to ingest streaming data with automated pattern identification
A data lake can be implemented as a complex configuration of data handling tools including Hadoop or other 
data storage systems, cluster services, data transformation, and data integration. These handlers have facilitated 
cross-infrastructure, analytic facilitation software to bring the configuration together.  
The risk of a data lake is that it can quickly become a data swamp – messy, unclean, and inconsistent. In order 
to establish an inventory of what is in a data lake, it is critical to manage Metadata as the data is ingested. In 
order to understand how the data in a data lake is associated or connected, data architects or data engineers often 
use unique keys or other techniques (semantic models, data models, etc.) so that data scientists and other 
visualization developers know how to use the information stored within the data lake. (See Chapter 9.)  
1.3.7 Services-Based Architecture 
Services-based architecture (SBA) is emerging as a way to provide immediate (if not completely accurate or 
complete) data, as well as update a complete, accurate historical data set, using the same source (Abate, Aiken, 
Burke, 1997). The SBA architecture is similar to the DW architectures which send data directly to an ODS for 
immediate access, as well as to the DW for historical accumulation. SBA architectures have three main 
components, a batch layer, a speed layer, and a serving layer. (See Figure 101.) 
•
Batch layer: A data lake serves as the batch layer, containing both recent and historical data
•
Speed layer: Contains only real-time data
•
Serving layer: Provides an interface to join data from the batch and speed layers
Data is loaded into both the batch and speed layers. All analytic computations are performed on data in both the 
batch and speed layers, which most likely requires implementation in two separate systems. Organizations 
address synchronization issues through trade-offs between completeness, latency, and complexity of merged 
views defined in the serving layer. Cost/benefit assessment is required to determine whether reducing latency or 
improving data completeness is worth the associated cost and complexity.  
The batch layer is often referred to as the structure-over-time component (here every transaction is an insert), 
whereas in the speed layer (often referred to as an Operational Data Store or ODS), all transactions are updates 
(or inserts only if required). In this manner, the architecture prevents synchronization issues while 
simultaneously creating a current state and a history layer. This architecture usually provides its data through a 
 

