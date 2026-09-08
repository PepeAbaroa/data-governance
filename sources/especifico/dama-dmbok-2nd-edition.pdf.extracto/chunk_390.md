# página 391 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA WAREHOUSING AND BUSINESS INTELLIGENCE • 387 
•
Operational Data Store (ODS): An ODS is integrated database of operational data. It may be sourced
directly from applications or from other databases. ODS’s generally contain current or near term data
(30-90 days), while a DW contains historical data as well (often several years of data). Data in ODS’s
is volatile, while warehouse data is stable. Not all organizations use ODS’s. They evolved as to meet
the need for low latency data. An ODS may serve as the primary source for a data warehouse; it may
also be used to audit a data warehouse.
•
Data marts: Data marts provide data prepared for analysis. This data is often a sub-set of warehouse
data designed to support particular kinds of analysis or a specific group of data consumers. For
example, marts can aggregate data to support faster analysis. Dimensional modeling (using
denormalization techniques) is often used to design user-oriented data marts.
•
Operational Data Mart (OpDM): An OpDM is a data mart focused on tactical decision support. It is
sourced directly from an ODS, rather than from a DW. It shares characteristics of the ODS: it contains
current or near-term data. Its contents are volatile.
•
Data Warehouse: The DW provides a single integration point for corporate data to support
management decision-making, and strategic analysis and planning. The data flows into a DW from the
application systems and ODS, and flows out to the data marts, usually in one direction only. Data that
needs correction is rejected, corrected at its source, and ideally re-fed through the system.
•
Operational reports: Reports are output from the data stores.
•
Reference, Master, and external data: In addition to transactional data from applications, the CIF
also includes data required to understand transactions, such as reference and Master Data. Access to
common data simplifies integration in the DW. While applications consume current master and
Reference Data, the DW also requires historical values and the timeframes during which they were
valid (see Chapter 10).
Figure 80 depicts movement within the CIF, from data collection and creation via applications (on the left) to 
the creation of information via marts and analysis (on the right). Movement from left to right includes other 
changes. For example,  
•
The purpose shifts from execution of operational functions to analysis
•
End users of systems move from front line workers to decision-makers
•
System usage moves from fixed operations to ad hoc uses
•
Response time requirements are relaxed (strategic decisions take more time than do daily operations)
•
Much more data is involved in each operation, query, or process
The data in DW and marts differs from that in applications: 
•
Data is organized by subject rather than function
•
Data is integrated data rather than ‘siloed’
•
Data is time-variant vs. current-valued only
•
Data has higher latency in DW than in applications
•
Significantly more historical data is available in DW than in applications
 

