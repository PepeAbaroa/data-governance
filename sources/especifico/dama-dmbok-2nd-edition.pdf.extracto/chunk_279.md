# página 280 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

276 • DMBOK2 
Data moving in batch mode will represent either the full set of data at a given point in time, such as account 
balances at the end of a period, or data that has changed values since the last time the data was sent, such as 
address changes that have been made in a day. The set of changed data is called the delta, and the data from a 
point in time is called a snapshot. 
With batch data integration solutions, there is often a significant delay between when data changes in the source 
and when it is updated in the target, resulting in high latency. Batch processing is very useful for processing 
very high volumes of data in a short time window. It tends to be used for data warehouse data integration 
solutions, even when lower latency solutions are available. 
To achieve fast processing and lower latency, some data integration solutions use micro-batch processing which 
schedules batch processing to run on a much higher frequency than daily, such as every five minutes. 
Batch data integration is used for data conversions, migrations, and archiving, as well as for extracting from and 
loading data warehouses and data marts. There are risks associated with the timing of batch processing. To 
minimize issues with application updates, schedule data movement between applications at the end of logical 
processing for the business day, or after special processing of the data has occurred at night. To avoid 
incomplete data sets, jobs moving data to a data warehouse should be scheduled based on the daily, weekly, or 
monthly reporting schedule. 
1.3.2.2 Change Data Capture 
Change Data Capture is a method of reducing bandwidth by filtering to include only data that has been changed 
within a defined timeframe. Change data capture monitors a data set for changes (inserts, changes, deletes) and 
then passes those changes (the deltas) to other data sets, applications, and organizations that consume the data. 
Data may also be tagged with identifiers such as flags or timestamps as part of the process. Change data capture 
may be data-based or log-based. (See Chapter 6.) 
There are three techniques for data-based change data capture. 
•
The source system populates specific data elements, such as timestamps within a range, or codes or
flags, which serve as change indicators. The extract process uses rules to identify rows to extract.
•
The source system processes add to a simple list of objects and identifiers when changing data, which
is then used to control selection of data for extraction.
•
The source system processes copy data that has changed into a separate object as part of the
transaction, which is then used for extract processing. This object does not need to be within the
database management system.
These types of extraction use capabilities built into the source application, which may be resource intensive and 
require the ability to modify the source application. 
 

