# página 292 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

288 • DMBOK2 
Analysis of lineage may identify updates required to documentation of systems in use. Custom-coded ETL and 
other legacy data manipulation objects should be documented to ensure that the organization can analyze the 
impact of any changes in the data flow.  
The analysis process may also identify opportunities for improvements in the existing data flow. For example, 
finding that code can be upgraded to a simple call to a function in a tool, or can be discarded as no longer 
relevant. Sometimes an old tool is performing a transformation that is undone later in the process. Finding and 
removing these inefficiencies can greatly help with the project’s success and with an organization’s overall 
ability to use its data.  
2.1.4 Profile Data 
Understanding data content and structure is essential to successful integration of data. Data profiling contributes 
to this end. Actual data structure and contents always differ from what is assumed. Sometimes differences are 
small; other times they are large enough to derail an integration effort. Profiling can help integration teams 
discover these differences and use that knowledge to make better decisions about sourcing and design. If data 
profiling is skipped, then information that should influence design will not be discovered until testing or 
operations.  
Basic profiling involves analysis of: 
•
Data format as defined in the data structures and inferred from the actual data
•
Data population, including the levels of null, blank, or defaulted data
•
Data values and how closely they correspond to a defined set of valid values
•
Patterns and relationships internal to the data set, such as related fields and cardinality rules
•
Relationships to other data sets
More extensive profiling of the potential source and target data sets is required to understand how well the data 
meets the requirements of the particular data integration initiative. Profile both the sources and targets to 
understand how to transform the data to match requirements. 
One goal of profiling is to assess the quality of data. Assessing the fitness of the data for a particular use 
requires documenting business rules and measuring how well the data meets those business rules. Assessing 
accuracy requires comparing to a definitive set of data that has been determined to be correct. Such data sets are 
not always available, so measuring accuracy may not be possible, especially as part of a profiling effort. 
As with high-level data discovery, data profiling includes verifying assumptions about the data against the 
actual data. Capture results of data profiling in a Metadata repository for use on later projects and use what is 
learned from the process to improve the accuracy of existing Metadata (Olson, 2003). (See Chapter 13.) 
The requirement to profile data must be balanced with an organization’s security and privacy regulations. (See 
Chapter 7.) 
 

