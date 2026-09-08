# página 517 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

BIG DATA AND DATA SCIENCE • 513 
Risks associated with data sources include privacy concerns. The ability to rapidly ingest and integrate data 
from a variety of sources at scale affords communities the ability to recombine data sets that were otherwise 
secured. Similarly, the published analysis may describe, through summary, aggregate, or modeled state, a sub-
set of the public that make it suddenly identifiable; this is a side effect of the ability to perform mass 
computation on very large populations, but publish to a very specific local or region. For example, when 
demographics computed at a national or country level quickly become non-identifiable, but not when published 
after filtering for a postal code or household level.92 
Criteria used to select or filter data also pose a risk. These criteria should be objectively managed to avoid 
biases or skews. Filtering can have a material impact on visualization. Discretion is necessary when removing 
outliers, restricting data sets to a limited domain, or dropping sparse elements. It is common practice to focus 
the provisioned data to emphasize isolation results, but it must be done objectively and uniformly.93 (See 
Chapter 2.) 
2.3 Acquire and Ingest Data Sources 
Once the sources are identified, they need to be found, sometimes purchased, and ingested (loaded) into the Big 
Data environment. During this process, capture critical Metadata about the source, such as its origin, size, 
currency, and additional knowledge about content. Many ingestion engines profile data as it is ingested, 
providing analysts with at least partial Metadata. Once the data is in a data lake, it can be assessed for suitability 
for multiple analysis efforts. Because building Data Science models is an iterative process, so is data ingestion. 
Iteratively identify gaps in the current data asset base and onboard those sources. Explore these data sources 
using profiling, visualization, mining, or other Data Science methods to define model algorithm inputs, or 
model hypotheses.  
Before integrating the data, assess its quality. Assessment can be as simple querying to find out how many 
fields contain null values, or as complex as running a data quality toolset or data analytic utility against the data 
to profile, classify, and identify relationships between data elements. Such assessment provides insight into 
whether the data provides a valid sample from which to work, and, if so, how the data can be stored and 
accessed (scattered across logical processing units [MPP], federated, distributed by key, etc.). This work 
involves SMEs (usually the data scientists themselves) and platform engineers.  
The assessment process provides valuable insight into how the data can be integrated with other data sets, such 
as Master Data or historical warehouse data. It also provides information that can be used in model training sets 
and validation activities.  
92 See Martin Fowler, Datensparsamkeit. Blog, 12 December 2013. Fowler brings into question the assumption that we 
should always capture as much data as possible. He points out that the “capture it all” approach brings up privacy risks. In 
its place, he puts forth the idea of data minimization or data sparsity (from the German term Datensparsamkeit) 
http://bit.ly/1f9Nq8K. 
93 For more information on the impact of bias, which can profoundly affect the interpretation of scientific results, consult the 
following websites: INFORMS is the leading international association for Operations Research and Analytics professionals. 
http://bit.ly/2sANQRW, Statistical Society of Canada: http://bit.ly/2oz2o5H and American Statistical Association: 
http://bit.ly/1rjAmHX. 
 

