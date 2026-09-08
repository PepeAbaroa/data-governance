# página 397 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA WAREHOUSING AND BUSINESS INTELLIGENCE • 393 
Another approach, the Data Vault, also cleanses and standardizes as part of the staging process. History is 
stored in a normalized atomic structure, dimensional surrogate, primary and alternate keys are defined. Ensuring 
that the business and surrogate key relationship remains intact becomes the secondary role of the vault – this is 
the data mart history. Facts persisted here as atomic structures. The vault is then available to a variety of data 
consumers via data marts. By retaining the history inside the vault, reloading facts is possible when later 
increments introduce grain changes. It is possible to virtualize the presentation layer, facilitating agile 
incremental delivery and collaborative development with the business community. A final materialization 
process can implement a more traditional star data mart for production end user consumption. 
1.3.8.2 Batch Change Data Capture 
Data Warehouses are often loaded daily and serviced by a nightly batch window. The load process can 
accommodate a variety of change detection, as each source system may require differing change capture 
techniques.  
Database log techniques are likely candidates for in-house developed applications as vendor purchased 
applications are unlikely to tolerate modification with triggers or additional overhead. Time stamped or log 
table loads are the most common. Full loads occur when dealing with legacy systems built without native time 
stamping capabilities (yes, there are applications without databases) or when certain batch recovery conditions 
apply. 
Table 28 summarizes difference between change data capture techniques, including their relative complexity 
and speed. The overlap column identifies whether there may be data duplication between source system changes 
and the target environment. When Overlap is ‘Yes’ this change data may already be present. When the Delete 
indicator is set to ‘Yes’ that the Change Data Method will track any deletes that have occurred in the source 
system – useful for expiring dimensions no longer in use. When Deletes are not tracked by the source system, 
additional efforts are required to determine when they occur. (See Chapter 8.) 
Table 28 CDC Technique Comparison 
Method 
Source System Requirement 
Complexity 
Fact 
Load 
Dimension 
Load 
Overlap 
Deletes 
Time 
stamped 
Delta Load 
Changes in the source system 
are stamped with the system date 
and time. 
Low 
Fast 
Fast 
Yes 
No 
Log Table 
Delta Load 
Source system changes are 
captured and stored in log tables 
Medium 
Nominal 
Nominal 
Yes 
Yes 
Database 
Transaction 
Log 
Database captures changes in the 
transaction log 
High 
Nominal 
Nominal 
No 
Yes 
Message 
Delta 
Source system changes are 
published as [near] real-time 
messages 
Extreme 
Slow 
Slow 
No 
Yes 
Full Load 
No change indicator, tables 
extracted in full and compared to 
identify change 
Simple 
Slow 
Nominal 
Yes 
Yes 
 

