# página 472 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

468 • DMBOK2 
•
Inconsistent business process execution: Data created through processes that are executed
inconsistently is likely to be inconsistent. Inconsistent execution may be due to training or
documentation issues as well as to changing requirements.
1.3.8.3 Issues Caused by Data Processing Functions 
•
Incorrect assumptions about data sources: Production issues can occur due to errors or changes,
inadequate or obsolete system documentation, or inadequate knowledge transfer (for example, when
SMEs leave without documenting their knowledge). System consolidation activities, such as those
associated with mergers and acquisitions, are often based on limited knowledge about the relationship
between systems. When multiple source systems and data feeds need to be integrated there is always a
risk that details will be missed, especially with varying levels of source knowledge available and tight
timelines.
•
Stale business rules: Over time, business rules change. They should be periodically reviewed and
updated. If there is automated measurement of rules, the technical process for measuring rules should
also be updated. If it is not updated, issues may not be identified or false positives will be produced (or
both).
•
Changed data structures: Source systems may change structures without informing downstream
consumers (both human and system) or without providing sufficient time to account for the changes.
This can result in invalid values or other conditions that prevent data movement and loading, or in
more subtle changes that may not be detected immediately.
1.3.8.4 Issues Caused by System Design 
•
Failure to enforce referential integrity: Referential integrity is necessary to ensure high quality data
at an application or system level. If referential integrity is not enforced or if validation is switched off
(for example, to improve response times), various data quality issues can arise:
o
Duplicate data that breaks uniqueness rules
o
Orphan rows, which can be included in some reports and excluded from others, leading to
multiple values for the same calculation
o
Inability to upgrade due to restored or changed referential integrity requirements
o
Inaccurate data due to missing data being assigned default values
•
Failure to enforce uniqueness constraints: Multiple copies of data instances within a table or file
expected to contain unique instances. If there are insufficient checks for uniqueness of instances, or if
the unique constraints are turned off in the database to improve performance, data aggregation results
can be overstated.
 

