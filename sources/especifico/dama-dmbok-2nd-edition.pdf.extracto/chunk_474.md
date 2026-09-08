# página 475 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA QUALITY • 471 
1.3.10.1 Data Cleansing 
Data Cleansing or Scrubbing transforms data to make it conform to data standards and domain rules. Cleansing 
includes detecting and correcting data errors to bring the quality of data to an acceptable level.  
It costs money and introduces risk to continuously remediate data through cleansing. Ideally, the need for data 
cleansing should decrease over time, as root causes of data issues are resolved. The need for data cleansing can 
be addressed by:  
•
Implementing controls to prevent data entry errors
•
Correcting the data in the source system
•
Improving the business processes that create the data
In some situations, correcting on an ongoing basis may be necessary, as re-processing the data in a midstream 
system is cheaper than any other alternative. 
1.3.10.2 Data Enhancement 
Data enhancement or enrichment is the process of adding attributes to a data set to increase its quality and 
usability. Some enhancements are gained by integrating data sets internal to an organization. External data can 
also be purchased to enhance organizational data (see Chapter 10). Examples of data enhancement include: 
•
Time/Date stamps: One way to improve data is to document the time and date that data items are
created, modified, or retired, which can help to track historical data events. If issues are detected with
the data, timestamps can be very valuable in root cause analysis, because they enable analysts to isolate
the timeframe of the issue.
•
Audit data: Auditing can document data lineage, which is important for historical tracking as well as
validation.
•
Reference vocabularies: Business specific terminology, ontologies, and glossaries enhance
understanding and control while bringing customized business context.
•
Contextual information: Adding context such as location, environment, or access methods and
tagging data for review and analysis.
•
Geographic information: Geographic information can be enhanced through address standardization
and geocoding, which includes regional coding, municipality, neighborhood mapping, latitude /
longitude pairs, or other kinds of location-based data.
•
Demographic information: Customer data can be enhanced through demographic information, such
as age, marital status, gender, income, or ethnic coding. Business entity data can be associated with
annual revenue, number of employees, size of occupied space, etc.
 

