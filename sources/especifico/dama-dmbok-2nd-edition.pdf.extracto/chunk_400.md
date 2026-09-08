# página 401 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA WAREHOUSING AND BUSINESS INTELLIGENCE • 397 
management systems. Chances are that tables and fields that contain equivalent data do not have the same 
names or structures.  
A solid taxonomy is necessary to map data elements in different systems to a consistent structure in the DW. 
Most often, this taxonomy is the logical data model. The mapping process must also address whether data in 
different structures is to be appended, changed in place, or inserted.  
2.3.2 Remediate and Transform Data 
Data remediation or cleansing activities enforce standards and correct and enhance the domain values of 
individual data elements. Remediation is particularly necessary for initial loads where significant history is 
involved. To reduce the complexity of the target system, source systems should be made responsible for data 
remediation and correction. 
Develop strategies for rows of data that are loaded but found to be incorrect. A policy for deleting old records 
may cause some havoc with related tables and surrogate keys, expiring a row and loading the new data as a 
completely new row may be a better option. 
An optimistic load strategy may include creating dimension entries to accommodate fact data. Such a process 
must account for how to update and expire such entries. Pessimistic load strategies should include a recycle area 
for fact data that cannot be associated with corresponding dimension keys. These entries require appropriate 
notification, alerting and reporting to ensure they are tracked, and reloaded later. Fact jobs should consider first 
loading recycled entries, then processing newly arrived content. 
Data transformation focuses on activities that implement business rules within a technical system. Data 
transformation is essential to data integration. Defining the correct rules by which to integrate data often 
requires direct involvement from Data Stewards and other SMEs. Rules should be documented so that they can 
be governed. Data integration tools perform these tasks. (See Chapter 8.) 
2.4 Populate the Data Warehouse 
The largest part of the work in any DW/BI effort is the preparation and processing of the data. The design 
decisions and principles for what data detail the DW contains are a key design priority for DW/BI architecture. 
Publishing clear rules for what data will be available via only operational reporting (such as in non-DW) is 
critical to the success of DW/BI efforts.  
The key factors to consider when defining a population approach are required latency, availability of sources, 
batch windows or upload intervals, target databases, dimensional aspects, and timeframe consistency of the data 
warehouse and data mart. The approach must also address data quality processing, time to perform 
transformations, and late-arriving dimensions and data rejects.  
 

