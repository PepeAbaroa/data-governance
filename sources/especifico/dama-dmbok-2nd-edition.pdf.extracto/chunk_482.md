# página 483 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA QUALITY • 479 
2.7.2 Measure and Monitor Data Quality 
The operational Data Quality Management procedures depend on the ability to measure and monitor the quality 
of data. There are two equally important reasons to implement operational data quality measurements: 
•
To inform data consumers about levels of quality
•
To manage risk that change may be introduced through changes to business or technical processes
Some measurements serve both purposes. Measurements should be developed based on findings from data 
assessment and root cause analysis. Measurements intended to inform data consumers will focus on critical data 
elements and relationships that, if they are not sound, will directly impact business processes. Measurements 
related to managing risk should focus on relationships that have gone wrong in the past and may go wrong in 
the future. For example, if data is derived based on a set of ETL rules and those rules may be impacted by 
changes to business processes, measurements should be put in place to detect changes to the data.  
Knowledge of past problems should be applied to manage risk. For example, if numerous data issues are 
associated with complex derivations, then all derivations should be assessed – even those that have not been 
associated with data issues. In most cases, it is worthwhile to put in place measurements that monitor functions 
similar to those that have had problems.  
Measurement results can be described at two levels: the detail related to the execution of individual rules and 
overall results aggregated from the rules. Each rule should have a standard, target, or threshold index for 
comparison. This function most often reflects the percentage of correct data or percentage of exceptions 
depending on the formula used. For example:  
𝑉𝑉𝑉𝑉𝑉𝑉𝑉𝑉𝑉𝑉𝑉𝑉𝑉𝑉𝑉𝑉(𝑟𝑟) = ൫𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇(𝑟𝑟) −𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸(𝑟𝑟)൯
𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇(𝑟𝑟)
𝐼𝐼𝐼𝐼𝐼𝐼𝐼𝐼𝐼𝐼𝐼𝐼𝐼𝐼𝐼𝐼𝐼𝐼𝐼𝐼(𝑟𝑟) = ൫𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸𝐸(𝑟𝑟)൯
𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑇𝑛𝑛𝑠𝑠(𝑟𝑟)
R represents the rule being tested. For example, 10,000 tests of a business rule (r) found 560 exceptions. In this 
example, the ValidDQ result would be 9440/10,000 = 94.4%, and the Invalid DQ result would be 560/10,000 = 
5.6%. 
Organizing the metrics and results as shown in Table 30 can help to structure measures, metrics, and indicators 
across the report, reveal possible rollups, and enhance communications. The report can be more formalized and 
linked to projects that will remediate the issues. Filtered reports are useful for data stewards looking for trends 
and contributions. Table 30 provides examples of rules constructed in this manner. Where applicable, results of 
rules are expressed in both positive percentages (the portion of the data that conforms to rules and expectations) 
and negative percentages (the portion of the data that does not conform to the rule).  
Data quality rules provide the foundation for operational management of data quality. Rules can be integrated 
into application services or data services that supplement the data lifecycle, either through Commercial Off The 
Shelf (COTS) data quality tools, rules engines and reporting tools for monitoring and reporting, or custom-
developed applications. 
 

