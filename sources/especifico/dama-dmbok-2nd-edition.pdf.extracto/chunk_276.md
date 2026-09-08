# página 277 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA INTEGRATION AND INTEROPERABILITY • 273 
1.3 Essential Concepts 
1.3.1 Extract, Transform, and Load 
Central to all areas in Data Integration and Interoperability is the basic process of Extract, Transform, and Load 
(ETL). Whether executed physically or virtually, in batch or real-time, these are the essential steps in moving 
data around and between applications and organizations. 
Depending on data integration requirements, ETL can be performed as a periodically scheduled event (batch) or 
whenever new or updated data is available (real-time or event-driven). Operational data processing tends to be 
real-time or near real-time, while data needed for analysis or reporting is often scheduled in batch jobs. 
Data integration requirements also determine whether the extracted and transformed data is physically stored in 
staging structures. Physical staging allows for an audit trail of steps that have occurred with the data and 
potential process restarts from an intermediate point. However, staging structures take up disk space and take 
time to write and read. Data integration needs that require very low latency will usually not include physical 
staging of the intermediate data integration results. 
1.3.1.1 Extract 
The extract process includes selecting the required data and extracting it from its source. Extracted data is then 
staged, in a physical data store on disk or in memory. If physically staged on disk, the staging data store may be 
co-located with the source data store or with the target data store, or both. 
Ideally, if this process executes on an operational system, it is designed to use as few resources as possible, in 
order to avoid negatively affecting the operational processes. Batch processing during off-peak hours is an 
option for extracts that include complex processing to perform the selection or identify changed data to extract. 
1.3.1.2 Transform 
The transform process makes the selected data compatible with the structure of the target data store. 
Transformation includes cases where data is removed from the source when it moves to the target, where data is 
copied to multiple targets, and where the data is used to trigger events but is not persisted.  
Examples of transformation may include 
•
Format changes: Conversion of the technical format of the data; for example, from EBCDIC to ASCII
format
•
Structure changes: Changes to the structure of the data; for example, from denormalized to
normalized records
 

