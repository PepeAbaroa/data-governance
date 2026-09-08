# página 403 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA WAREHOUSING AND BUSINESS INTELLIGENCE • 399 
offer embedded analytics with standard content fetched from pre-populated cubes or aggregate tables. 
Virtualization has blurred the lines between on-premises data sources and external purchased or open data, and 
in some cases provisions user-controlled report-centric integration on demand. In other words, it is prudent for 
companies to use common infrastructure and delivery mechanisms. These include the web, email, and 
applications for the delivery of all kinds of information and reports, of which DW/BI is a subset. 
Many vendors are now combining related BI Tools, through mergers and acquisitions or net new development, 
and offering BI Suites. Suites are the primary option at the Enterprise Architecture level but given that most 
organizations have already purchased individual tools, or embraced open source tools, questions around 
replacement versus co-existence are likely to surface. Remember that every BI tool comes with a price, 
requiring system resources, support, training, and architectural integration. 
2.6 Maintain Data Products 
An implemented warehouse and its customer-facing BI tools is a data product. Enhancements (extensions, 
augmentations, or modifications) to an existing DW platform should be implemented incrementally.  
Maintaining the scope for an increment, and executing a critical path for key work items, can be a challenge in a 
dynamic work environment. Set priorities with business partners and focus work on mandatory enhancements.  
2.6.1 Release Management 
Release Management is critical to an incremental development processes that grows new capabilities, enhances 
the production deployment, and ensures provision of regular maintenance across the deployed assets. This 
process will keep the warehouse up-to-date, clean, and operating at its best. However, this process requires the 
same alignment between IT and Business as between the Data Warehouse model and the BI capabilities. It is a 
continual improvement effort.  
Figure 83 illustrates an example release process, based on a quarterly schedule. Over the year, there are three 
business-driven releases and one technology-based release (to address requirements internal to the warehouse). 
The process should enable incremental development of the warehouse and management of the backlog of 
requirements.  
2.6.2 Manage Data Product Development Lifecycle 
While data consumers are using the existing DW, the DW team is preparing for the next iteration, with the 
understanding that not all items will go to production. Align the iterations to releases with a backorder work list 
prioritized by the business units. Each iteration will extend an existing increment or add new functionality by 
onboarding a business unit. Releases will align functionality to the business unit, whereas the iteration will align 
the functionality to the configuration itself managed by the product manager.  
 

