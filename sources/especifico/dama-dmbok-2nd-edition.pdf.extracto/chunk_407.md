# página 408 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

404 • DMBOK2 
customer-level capabilities. BI tools are evolving quickly, enabling a transition from IT-led, standardized 
reporting to self-service, business-driven data exploration.69 
•
Operational reporting is the application of BI tools to analyze business trends, both short-term
(month-over-month) and longer-term (year-over-year). Operational reporting can also help discover
trends and patterns. Use Tactical BI to support short-term business decisions.
•
Business performance management (BPM) includes the formal assessment of metrics aligned with
organizational goals. This assessment usually happens at the executive level. Use Strategic BI to
support long-term corporate goals and objectives.
•
Descriptive, self-service analytics provides BI to the front lines of the business, where analytical
capabilities guide operational decisions. Operational analytics couples BI applications with operational
functions and processes, to guide decisions in near-real-time. The requirement for low latency (near
real-time data capture and data delivery) will drive the architectural approach to operational analytics
solutions. Service-oriented Architecture (SOA) and Big Data become necessary to support operational
analytics fully (see Chapters 8 and 15).
3.3.1 Operational Reporting 
Operational Reporting involves business users generating reports directly from transactional systems, 
operational applications, or a data warehouse. This is typically an application functionality. Often business areas 
will start to use a DW for operational reporting, especially if DW/BI governance is poor, or the DW contains 
additional data that enhances the operational, transaction data. Often the reports will appear as ad-hoc queries, 
when in fact they are simple reports or are used to initiate workflow. From a data management perspective, the 
key is to understand if the data necessary for this reporting exists within the application itself, or if it requires 
data enhancements from the DW or operational data store. 
Data exploration and reporting tools, sometimes called ad-hoc query tools, enable users to author their own 
reports or create outputs for use by others. They are less concerned with the precise layout because they are not 
trying to generate an invoice or the like. However, they do want to include charts and tables quickly and 
intuitively. Often the reports created by business users become standard reports, not exclusively used for ad hoc 
business questions. 
The needs within business operations reporting are often different from the needs within business query and 
reporting. With business query and reporting, the data source is usually a data warehouse or data mart (though 
not always). While IT develops production reports, power users and ad hoc business users develop their own 
reports with business query tools. Use reports generated with business query tools individually, departmentally, 
or enterprise-wide. 
69 Dataversity refers to this trend as the “democratization of data technologies.” See Ghosh, Paramita. “A Comparative 
Study of Business Intelligence and Analytics Market Trends.” Dataversity. January 17, 2017. http://bit.ly/2sTgXTJ 
(accessed 2017-01-22). 
 

