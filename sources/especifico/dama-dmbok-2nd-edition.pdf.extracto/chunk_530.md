# página 531 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

BIG DATA AND DATA SCIENCE • 527 
even the source filesystems. Consideration of real-time feeds versus data at rest versus computational data 
elements is necessary to complete the source side lineage.  
6.5 Data Quality 
Data Quality is a measure of deviation from an expected result: the smaller the difference, the better the data 
meets expectation, and the higher the quality. In an engineered environment, standards for quality should be 
easy to define (though practice shows that they are not or that many organizations do not take the time to define 
them). Some people have raised the question of whether data quality even matters for Big Data. Common sense 
says it does. For analytics to be reliable, the underlying data must be reliable. In Big Data projects, it may seem 
very difficult to determine the quality of data, but an effort needs to be made to assess quality in order to have 
confidence in the analysis. This can be done through an initial assessment, which is necessary to understand the 
data, and through that, the identification of measurements for subsequent instances of the data set. Data quality 
assessment will produce valuable Metadata that will be necessary input to any effort to integrate data.  
Consider that most mature Big Data organizations scan data input sources using data quality toolsets to 
understand the information contained within. Most advanced data quality toolsets offer functionality that 
enables an organization to test assumptions and build knowledge about its data. For example:  
•
Discovery: Where information resides within the data set
•
Classification: What types of information are present based upon standardized patterns
•
Profiling: How the data is populated and structured
•
Mapping: What other data sets can be matched to these values
Just as in DW/BI, it is tempting to put data quality assessment last. Without it, though, it may be difficult to 
know what Big Data represents or how to make connections between data sets. Integration will be necessary, 
and the likelihood that data feeds will be provisioned with identical structures and elements is very nearly zero. 
This means for example, codes and other potential linking data will likely vary from data provider to data 
provider. Without initial assessment, such conditions will go unnoticed until an analytic need is expressed that 
attempts to merge or combine those providers. 
6.6 Metrics 
Metrics are vital to any management process; they not only quantify activity, but can define the variation 
between what is observed and what is desired.  
6.6.1 Technical Usage Metrics 
Many of the Big Data tools offer insightful administrator reporting capabilities that interact directly with the 
contents queried by the user community. Technical usage analysis looks for data hot spots (most frequently 
 

