# página 474 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

470 • DMBOK2 
These changes are generally NOT undo-able without a complete restore from backup as there is only the 
database log to show the changes. Therefore, these shortcuts are strongly discouraged – they are opportunities 
for security breaches and business disruption longer than a proper correction would cause. All changes should 
go through a governed change management process.  
1.3.9 Data Profiling 
Data Profiling is a form of data analysis used to inspect data and assess quality. Data profiling uses statistical 
techniques to discover the true structure, content, and quality of a collection of data (Olson, 2003). A profiling 
engine produces statistics that analysts can use to identify patterns in data content and structure. For example:  
•
Counts of nulls: Identifies nulls exist and allows for inspection of whether they are allowable or not
•
Max/Min value: Identifies outliers, like negatives
•
Max/Min length: Identifies outliers or invalids for fields with specific length requirements
•
Frequency distribution of values for individual columns: Enables assessment of reasonability (e.g.,
distribution of country codes for transactions, inspection of frequently or infrequently occurring values,
as well as the percentage of the records populated with defaulted values)
•
Data type and format: Identifies level of non-conformance to format requirements, as well as
identification of unexpected formats (e.g., number of decimals, embedded spaces, sample values)
Profiling also includes cross-column analysis, which can identify overlapping or duplicate columns and expose 
embedded value dependencies. Inter-table analysis explores overlapping values sets and helps identify foreign 
key relationships. Most data profiling tools allow for drilling down into the analyzed data for further 
investigation.  
Results from the profiling engine must be assessed by an analyst to determine whether data conforms to rules 
and other requirements. A good analyst can use profiling results to confirm known relationships and uncover 
hidden characteristics and patterns within and between data sets, including business rules, and validity 
constraints. Profiling is usually used as part of data discovery for projects (especially data integration projects; 
see Chapter 8) or to assess the current state of data that is targeted for improvement. Results of data profiling 
can be used to identify opportunities to improve the quality of both data and Metadata (Olson, 2003; 
Maydanchik, 2007). 
While profiling is an effective way to understand data, it is just a first step to data quality improvement. It 
enables organizations to identify potential problems. Solving problems requires other forms of analysis, 
including business process analysis, analysis of data lineage, and deeper data analysis that can help isolate root 
causes of problems.  
1.3.10 Data Quality and Data Processing  
While the focus of data quality improvement efforts is often on the prevention of errors, data quality can also be 
improved through some forms of data processing. (See Chapter 8.)  
 

