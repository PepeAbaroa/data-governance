# página 530 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

526 • DMBOK2 
•
Processes for neutral and expert presentation to avoid biased results, and to ensure that all elements
included have been done so in a fair and consistent manner including:
o
Data inclusion and exclusion
o
Assumptions in the models
o
Statistical validity of results
o
Validity of interpretation of results
o
Appropriate methods applied
6.3 Data Security 
Having a reliable process to secure data is itself an organizational asset. Policies for handling and securing Big 
Data should be established and monitored. These policies should account for how to prevent misuse of personal 
data and to secure it through its overall lifecycle.  
Securely provision appropriate levels of data for authorized personnel and make subscription data accessible 
according to agreed-upon levels. Align services to user communities so that special services can be created to 
provision private data for those communities allowed to ingest it, and mask the data for others. Often 
organizations create policies for access to information that are not to be violated (such as no access by name, 
address, or phone number). In order to secure information that is highly sensitive (social security number, credit 
card numbers, etc.), data will be stored using encryption techniques that obfuscate the information. Encryption 
can be chosen that, for example, has the same ‘content’ when encrypted, so that patterns may be exposed 
without knowing the actual values. 
Recombination measures the ability to reconstitute sensitive or private data. This capability must be managed as 
part of the Big Data security practice. The outcomes of the analysis may violate privacy, even though the actual 
data elements can only be inferred. Understanding the outcomes at the Metadata Management level is critical to 
avoid this and other potential security violations. This requires knowledge of the intended consumption or 
analysis to be performed and by what role. Some trusted persons within the organization will be granted the 
ability to read this data when necessary, but not everyone, and certainly not for deep analysis. (See Chapters 2 
and 7.) 
6.4 Metadata 
As part of a Big Data initiative, an organization will bring together data sets that were created using different 
approaches and standards. Integration of such data is challenging. Metadata related to these data sets is critical 
to their successful use. Metadata needs to be carefully managed as part of data ingestion, or the data lake will 
quickly become a data swamp. The user community must have tools that enable them to create a master list of 
data sets with Metadata that characterizes the structure, content, and quality of the data, including the source 
and lineage of the data and the definition and intended uses of entities and data elements. Technical Metadata 
can be harvested from a variety of Big Data tools including data storage layers, data integration, MDM, and 
 

