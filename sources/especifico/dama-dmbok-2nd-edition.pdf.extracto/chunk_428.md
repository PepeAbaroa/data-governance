# página 429 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

METADATA MANAGEMENT • 425 
entries; record keeping Metadata, such as retention policies; and preservation Metadata, such as storage, 
archival condition, and rules for conservation. (See Chapter 9.) 
While most assertions about Metadata for unstructured data are connected to traditional content management 
concerns, new practices are emerging around managing unstructured data in data lakes. Organizations wanting 
to take advantage of data lakes, using Big Data platforms such as Hadoop, are finding that they must catalog 
ingested data in order to enable later access. Most put in place processes to collect Metadata as part of data 
ingestion. A minimum set of Metadata attributes needs to be collected about each object ingested in the data 
lake (e.g., name, format, source, version, date received, etc.). This produces a catalog of data lake contents.  
1.3.5 Sources of Metadata 
As should be clear from the types of Metadata, Metadata can be collected from many different sources. 
Moreover, if Metadata from applications and databases has been well-managed, it can simply be harvested and 
integrated. However, most organizations do not manage Metadata well at the application level, because 
Metadata is often created as a by-product of application processing rather than as an end product (i.e., it is not 
created with consumption in mind). As with other forms of data, there is a lot of work in preparing Metadata 
before it can be integrated.  
The majority of operational Metadata is generated as data is processed. The key to using this Metadata is to 
collect it in a usable form, and to ensure that those responsible for interpreting it have the tools they need to do 
so. Keep in mind that interpreting data in places like error logs itself requires Metadata that describes the logs. 
Similarly, a large portion of technical Metadata can be harvested from database objects.  
It is possible to reverse engineer knowledge about data from existing systems and to harvest business Metadata 
from existing data dictionaries, models, and process documentation (Loshin, 2001; Aiken, 1995), but there are 
risks in doing so. The biggest risk is not knowing how much care was taken to develop and refine the 
definitions in the first place. If definitions are underdeveloped or ambiguous, then they will not provide data 
consumers with the information they need to understand the data they are using.  
It is better to be intentional about developing definitions than to simply accept existing ones. Development of 
definitions takes time and the right skill set (e.g., writing and facilitation skills). This is why the development of 
business Metadata requires stewardship. (See Chapter 3.)  
Much of the technical Metadata required to manage databases and the business Metadata required to use data 
can be collected and developed as part of project work. For example, the process of modeling data requires 
discussions on the meaning of data elements and the relation between them. Knowledge shared during such 
discussions should be captured and groomed for use in Data Dictionaries, Business Glossaries, and other 
repositories. The data models themselves include important details about the physical characteristics of data. 
Time should be allocated to ensure that project artifacts contain high quality Metadata that aligns with 
enterprise standards.  
 

