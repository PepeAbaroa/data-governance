# página 405 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA WAREHOUSING AND BUSINESS INTELLIGENCE • 401 
Items passing the pilot and deemed production-ready by both business and IT representatives can be promoted 
to production as new data products. This completes one iteration.  
Items not passing pilot can be rejected entirely or returned to development for fine-tuning. Perhaps additional 
support from the DW team is needed at this time to advance the item in the next promotion iteration.  
2.6.3 Monitor and Tune Load Processes 
Monitor load processing across the system for bottlenecks and dependencies. Employ database tuning 
techniques where and when needed, including partitioning, tuned backup, and recovery strategies. Archiving is 
a difficult subject in data warehousing.  
Users often consider the data warehouse as an active archive due to the long histories that are built and are 
unwilling, particularly if the On Line Analytical Processing (OLAP) sources have dropped records, to see the 
data warehouse engage in archiving. (See Chapter 6.) 
2.6.4 Monitor and Tune BI Activity and Performance 
A best practice for BI monitoring and tuning is to define and display a set of customer-facing satisfaction 
metrics. Average query response time and the number of users per day, week, or month are examples of useful 
metrics. In addition to the statistical measures available from the systems, it is useful to survey DW/BI 
customers regularly. 
Regular review of usage statistics and patterns is essential. Reports providing frequency and resource usage of 
data, queries, and reports allow prudent enhancement. Tuning BI activity is analogous to the principle of 
profiling applications in order to know where the bottlenecks are and where to apply optimization efforts. The 
creation of indexes and aggregations is most effective when done according to usage patterns and statistics. 
Tremendous performance gains can come from simple solutions such as posting the completed daily results to a 
report that runs hundreds or thousands of times a day. 
Transparency and visibility are the key principles that should drive DW/BI monitoring. The more one can 
expose the details of the DW/BI activities, the more data consumers can see and understand what is going on 
(and have confidence in the BI), and less direct end-customer support will be required. Providing a dashboard 
that exposes the high-level status of data delivery activities, with drill-down capability, is a best practice that 
allows an on-demand-pull of information by both support personnel and customers.  
The addition of data quality measures will enhance the value of this dashboard where performance is more than 
just speed and timing. Use heat maps to visualize workload on infrastructure, data throughput, and compliance 
to operating agreement levels. 
 

