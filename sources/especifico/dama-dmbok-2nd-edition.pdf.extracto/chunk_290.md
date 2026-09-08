# página 291 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA INTEGRATION AND INTEROPERABILITY • 287 
Data integration and lifecycle requirements are usually defined by business analysts, data stewards, and 
architects in various functions, including IT, who have a desire to get data in a certain place, in a certain format, 
and integrated with other data. The requirements will determine the type of DII interaction model, which then 
determines the technology and services necessary to fulfill the requirements. 
The process of defining requirements creates and uncovers valuable Metadata. This Metadata should be 
managed throughout the data lifecycle, from discovery through operations. The more complete and accurate an 
organization’s Metadata, the better its ability to manage the risks and costs of data integration.  
2.1.2 Perform Data Discovery 
Data discovery should be performed prior to design. The goal of data discovery is to identify potential sources 
of data for the data integration effort. Discovery will identify where data might be acquired and where it might 
be integrated. The process combines a technical search, using tools that scan the Metadata and/or actual 
contents on an organization’s data sets, with subject matter expertise (i.e., interviewing people who work with 
the data of interest). 
Discovery also includes high-level assessment of data quality, to determine whether the data is fit for the 
purposes of the integration initiative. This assessment requires not only reviewing existing documentation, 
interviewing subject matter experts, but also verifying information gathered against the actual data through data 
profiling or other analysis. (See Section 2.1.4.) In almost all cases, there will be discrepancies between what is 
believed about a data set and what is actually found to be true. 
Data discovery produces or adds to an inventory of organizational data. This inventory should be maintained in 
a Metadata repository. Ensure this inventory is maintained as a standard part of integration efforts: add or 
remove data stores, document structure changes.  
Most organizations have a need to integrate data from their internal systems. However, data integration 
solutions may also involve the acquisition of data from outside the organization. There is a vast and ever 
growing amount of valuable information available for free, or from data vendors. Data from external sources 
can be extremely valuable when integrated with data from within an organization. However, acquiring and 
integrating external data takes planning.  
2.1.3 Document Data Lineage 
The process of data discovery will also uncover information about how data flows through an organization. This 
information can be used to document high-level data lineage: how the data under analysis is acquired or created 
by the organization, where it moves and is changed within the organization, and how the data is used by the 
organization for analytics, decision-making, or event triggering. Detailed lineage can include the rules 
according to which data is changed, and the frequency of changes.  
 

