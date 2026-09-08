# página 416 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

412 • DMBOK2 
systems over the initial load, and after a few update load cycles, to meet sign-off criteria. Meeting these 
requirements is paramount for every DW/BI implementation. Consider, up-front, a few critically important 
architectural sub-components, along with their supporting activities: 
•
Conceptual Data Model: What information is core to the organization? What are the key business
concepts and how are they related to each other?
•
Data quality feedback loop: How are data issues identified and remediated? How are owners of the
systems in which issues originate informed about problems and held accountable for fixing them?
What is the remediation process for issues that are caused by the DW data integration processes?
•
End-to-end Metadata: How does the architecture support the integrated end-to-end flow of Metadata?
In particular, is access to meaning and context designed into the architecture? How do data consumers
answer basic questions like "What does this report mean?" or "What does this metric mean?"
•
End-to-end verifiable data lineage: Are the items exposed to business users traceable to the source
systems in an automated, maintained manner? Is a system of record identified for all data?
6.2 Customer / User Satisfaction 
Perceptions of the quality of data will drive customer satisfaction but satisfaction is dependent on other factors 
as well, such as data consumers’ understanding of the data and the operations team’s responsiveness to 
identified issues. Collecting, understanding, and acting on customer feedback can be facilitated through 
regularly scheduled meetings with user representatives. Such interaction can also help the warehouse team share 
information about the release roadmap and understand how data consumers are using the warehouse.  
6.3 Service Level Agreements 
Business and technical expectations for the environments should be specified in Service Level Agreements 
(SLAs). Often the response time, data retention, and availability requirements differ greatly between classes of 
business needs and their respective supporting systems (e.g., ODS versus DW versus data mart). 
6.4 Reporting Strategy 
Ensure that a reporting strategy exists within and across the BI Portfolio. A reporting strategy includes 
standards, processes, guidelines, best practices, and procedures. It will ensure users have clear, accurate, and 
timely information. The reporting strategy must address  
•
Security access to ensure that only entitled users will gain access to sensitive data elements
•
Access mechanisms to describe how users want to interact, report, examine or view their data
 

