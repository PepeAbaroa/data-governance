# página 293 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA INTEGRATION AND INTEROPERABILITY • 289 
2.1.5 Collect Business Rules 
Business rules are a critical subset of requirements. A business rule is a statement that defines or constrains an 
aspect of business processing. Business rules are intended to assert business structure or to control or influence 
the behavior of the business. Business rules fall into one of four categories: definitions of business terms, facts 
relating terms to each other, constraints or action assertions, and derivations. 
Use business rules to support Data Integration and Interoperability at various points, to: 
•
Assess data in potential source and target data sets
•
Direct the flow of data in the organization
•
Monitor the organization’s operational data
•
Direct when to automatically trigger events and alerts
For Master Data Management, business rules include match rules, merge rules, survivorship rules, and trust 
rules. For data archiving, data warehousing, and other situations where a data store is in use, the business rules 
also include data retention rules. 
Gathering business rules is also called rules harvesting or business rule mining. The business analyst or data 
steward can extract the rules from existing documentation (like use cases, specifications, or system code), or 
they may also organize workshops and interviews with subject matter experts (SMEs), or both. 
2.2 Design Data Integration Solutions 
2.2.1 Design Data Integration Architecture 
Data integration solutions should be specified at both the enterprise level and the individual solution level (see 
Chapter 4). By establishing enterprise standards, the organization saves time in implementing individual 
solutions, because assessments and negotiations have been performed in advance of need. An enterprise 
approach saves money in the cost of licenses through group discounts and in the costs of operating a consistent 
and less complex set of solutions. Operational resources that support and back up one another can be part of a 
shared pool. 
Design a solution to meet the requirements, reusing as many of the existing Data Integration and 
Interoperability components as is feasible. A solution architecture indicates the techniques and technologies that 
will be used. It will include an inventory of the involved data structures (both persistent and transitive, existing 
and required), an indication of the orchestration and frequency of data flow, regulatory and security concerns 
and remediation, and operating concerns around backup and recovery, availability, and data archive and 
retention. 
 

