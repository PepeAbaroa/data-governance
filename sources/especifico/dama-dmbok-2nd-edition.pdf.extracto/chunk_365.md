# página 366 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

362 • DMBOK2 
Planning for, evaluating, and incorporating new data sources into the Master Data Management solution must 
be a reliable, repeatable process. Data acquisition activities involve: 
•
Receiving and responding to new data source acquisition requests
•
Performing rapid, ad-hoc, match and high-level data quality assessments using data cleansing and data
profiling tools
•
Assessing and communicating complexity of data integration to the requesters to help them with their
cost-benefit analysis
•
Piloting acquisition of data and its impact on match rules
•
Finalizing data quality metrics for the new data source
•
Determining who will be responsible for monitoring and maintaining the quality of a new source’s data
•
Completing integration into the overall data management environment
1.3.3.4.3 Data Validation, Standardization, and Enrichment 
To enable entity resolution, data must be made as consistent as possible. This entails, at a minimum, reducing 
variation in format and reconciling values. Consistent input data reduces the chance or errors in associating 
records. Preparation processes include:  
•
Validation: Identifying data prove-ably erroneous or likely incorrect or defaulted (for example,
removal of clearly fake email addresses)
•
Standardization: Ensuring data content conforms to standard Reference Data values (e.g., country
codes), formats (e.g., telephone numbers) or fields (e.g., addresses)
•
Enrichment: Adding attributes that can improve entity resolution services (e.g., Dunn and Bradstreet
DUNS Number and Ultimate DUNS Number for relating company records, Acxiom or Experian
Consumer IDs for individual records)
Table 25 illustrates the results of the cleansing and standardization process on the example from Table 24. 
Addresses that had had different formats are now recognizably the same. Phone numbers include standard 
formatting. 
Table 25 Standardized and Enriched Input Data 
Source ID 
Name 
Address (Cleansed) 
Telephone (Cleansed) 
123 
John Smith 
123 Main, Dataland, SQ 98765 
234 
J. Smith 
123 Main, Dataland, SQ 98765 
 +1 234 567 8900 
345 
Jane Smith 
123 Main, Dataland, SQ 98765 
+1 234 567 8900 
1.3.3.4.4 Entity Resolution and Identifier Management 
Entity resolution is the process of determining whether two references to real world objects refer to the same 
object or to different objects (Talburt, 2011). Entity resolution is a decision-making process. Models for 
 

