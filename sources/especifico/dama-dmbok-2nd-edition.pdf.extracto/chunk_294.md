# página 295 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA INTEGRATION AND INTEROPERABILITY • 291 
Transformation may be performed on a batch schedule, or triggered by the occurrence of a real-time event. It 
may be accomplished through physical persistence of the target format or through virtual presentation of the 
data in the target format. 
2.2.4 Design Data Orchestration 
The flow of data in a data integration solution must be designed and documented. Data orchestration is the 
pattern of data flows from start to finish, including intermediate steps, required to complete the transformation 
and/or transaction.  
Batch data integration orchestration will indicate the frequency of the data movement and transformation. Batch 
data integration is usually coded into a scheduler that triggers the start at a certain time, periodicity, or when an 
event occurs. The schedule may include multiple steps with dependencies.  
Real-time data integration orchestration is usually triggered by an event, such as new or updated data. Real-time 
data integration orchestration is usually more complex and implemented across multiple tools. It may not be 
linear in nature. 
2.3 Develop Data Integration Solutions 
2.3.1 Develop Data Services 
Develop services to access, transform, and deliver data as specified, matching the interaction model selected. 
Tools or vendor suites are most frequently used to implement data integration solutions, such as data 
transformation, Master Data Management, data warehousing, etc. Using consistent tools or standard vendor 
suites across the organization for these various purposes can simplify operational support and lower operating 
costs by enabling shared support solutions. 
2.3.2 Develop Data Flows 
Integration or ETL data flows will usually be developed within tools specialized to manage those flows in a 
proprietary way. Batch data flows will be developed in a scheduler (usually the enterprise standard scheduler) 
that will manage the order, frequency, and dependency of executing the data integration pieces that have been 
developed.  
Interoperability requirements may include developing mappings or coordination points between data stores. 
Some organizations use an ESB to subscribe to data that is created or changed in the organization and other 
applications to publish changes to data. The enterprise service bus will poll the applications constantly to see if 
they have any data to publish and deliver to them new or changed data for which they have subscribed. 
 

