# página 473 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA QUALITY • 469 
•
Coding inaccuracies and gaps: If the data mapping or layout is incorrect, or the rules for processing
the data are not accurate, the data processed will have data quality issues, ranging from incorrect
calculations to data being assigned to or linked to improper fields, keys, or relationships.
•
Data model inaccuracies: If assumptions within the data model are not supported by the actual data,
there will be data quality issues ranging from data loss due to field lengths being exceeded by the
actual data, to data being assigned to improper IDs or keys.
•
Field overloading: Re-use of fields over time for different purposes, rather than changing the data
model or code can result in confusing sets of values, unclear meaning, and potentially, structural
problems, like incorrectly assigned keys.
•
Temporal data mismatches: In the absence of a consolidated data dictionary, multiple systems could
implement disparate date formats or timings, which in turn lead to data mismatch and data loss when
data synchronization takes place between different source systems.
•
Weak Master Data Management: Immature Master Data Management can lead to choosing
unreliable sources for data, which can cause data quality issues that are very difficult to find until the
assumption that the data source is accurate is disproved.
•
Data duplication: Unnecessary data duplication is often a result of poor data management. There are
two main types of undesirable duplication issues:
o
Single Source – Multiple Local Instances: For example, instances of the same customer in
multiple (similar or identical) tables in the same database. Knowing which instance is the
most accurate for use can be difficult without system-specific knowledge.
o
Multiple Sources – Single Instance: Data instances with multiple authoritative sources or
systems of record. For example, single customer instances coming from multiple point-of-sale
systems. When processing this data for use, there can be duplicate temporary storage areas.
Merge rules determine which source has priority over others when processing into permanent
production data areas.
1.3.8.5 Issues Caused by Fixing Issues 
Manual data patches are changes made directly on the data in the database, not through the business rules in the 
application interfaces or processing. These are scripts or manual commands generally created in a hurry and 
used to ‘fix’ data in an emergency such as intentional injection of bad data, lapse in security, internal fraud, or 
external source for business disruption.  
Like any untested code, they have a high risk of causing further errors through unintended consequences, by 
changing more data than required, or not propagating the patch to all historical data affected by the original 
issue. Most such patches also change the data in place, rather than preserving the prior state and adding 
corrected rows.  
 

