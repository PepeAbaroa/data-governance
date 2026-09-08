# página 389 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA WAREHOUSING AND BUSINESS INTELLIGENCE • 385 
An Enterprise Data Warehouse (EDW) is a centralized data warehouse designed to service the BI needs of the 
entire organization. An EDW adheres to an enterprise data model to ensure consistency of decision support 
activities across the enterprise. 
1.3.3 Data Warehousing 
Data Warehousing describes the operational extract, cleansing, transformation, control, and load processes that 
maintain the data in a data warehouse. The data warehousing process focuses on enabling an integrated and 
historical business context on operational data by enforcing business rules and maintaining appropriate business 
data relationships. Data warehousing also includes processes that interact with Metadata repositories. 
Traditionally, data warehousing focuses on structured data: elements in defined fields, whether in files or tables, 
as documented in data models. With recent advances in technology, the BI and DW space now embraces semi-
structured and unstructured data. Semi-structured data, defined as electronic elements organized as semantic 
entities with no required attribute affinity, predates XML but not HTML; an EDI transfer could serve as an 
example. Unstructured data refers to data that is not predefined through a data model. Because unstructured data 
exists in a range of formats and encompasses items such as e-mail, free format text, business documents, videos, 
photos, and web pages to name a few, defining a feasible storage construct that sustains analytic workloads 
within warehousing governance has been a challenge yet to be overcome. 
1.3.4 Approaches to Data Warehousing 
Much of the conversation about what constitutes a data warehouse has been driven by two influential thought 
leaders – Bill Inmon and Ralph Kimball – who have different approaches to modeling and developing 
warehouses. Inmon defines a data warehouse as “a subject-oriented, integrated, time-variant and non-volatile 
collection of data in support of management’s decision-making process.”64 A normalized relational model is 
used to store and manage data. Kimball defines a warehouse as “a copy of transaction data specifically 
structured for query and analysis.” Kimball’s approach calls for a dimensional model. (See Chapter 5.) 
While Inmon and Kimball advocate different approaches to building warehouses, their definitions recognize 
similar core ideas: 
•
Warehouses store data from other systems
•
The act of storage includes organizing the data in ways that increase its value
•
Warehouses make data accessible and usable for analysis
•
Organizations build warehouses because they need to make reliable, integrated data available to
authorized stakeholders
•
Warehouse data serves many purposes, from support of workflow to operational management to
predictive analytics
64 http://bit.ly/1FtgeIL, last accessed 2/27/2016. 
 

