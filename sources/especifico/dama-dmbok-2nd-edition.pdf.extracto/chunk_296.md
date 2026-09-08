# página 297 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA INTEGRATION AND INTEROPERABILITY • 293 
Preparation and pre-processing of the historical data needed in the predictive model may be performed in 
nightly batch processes or in near real-time. Usually some of the predictive model can be populated in advance 
of the triggering event, such as identifying what products are usually bought together in preparation of 
suggesting an additional item for purchase. 
Some processing flows trigger a response to every event in the real-time stream, such as adding an item to a 
shopping cart; other processing flows attempt to identify particularly meaningful events that trigger action, such 
as a suspected fraudulent charge attempt on a credit card. 
The response to the identification of a meaningful event may be as simple as a warning being sent out or as 
complex as the automatic deployment of armed forces. 
2.3.6 Maintain DII Metadata 
As previously noted (see Section 2.1), an organization will create and uncover valuable Metadata during the 
process of developing DII solutions. This Metadata should be managed and maintained to ensure proper 
understanding of the data in the system, and to prevent the need to rediscover it for future solutions. Reliable 
Metadata improves an organization’s ability to manage risks, reduce costs, and obtain more value from its data.  
Document the data structures of all systems involved in data integration as source, target, or staging. Include 
business definitions and technical definitions (structure, format, size), as well as the transformation of data 
between the persistent data stores. Whether data integration Metadata is stored in documents or a Metadata 
repository, it should not be changed without a review and approval process from both business and technical 
stakeholders.  
Most ETL tool vendors package their Metadata repositories with additional functionality that enables 
governance and stewardship oversight. If the Metadata repository is utilized as an operational tool, then it may 
even include operational Metadata about when data was copied and transformed between systems. 
Of particular importance for DII solutions is the SOA registry, which provides controlled access to an evolving 
catalog of information about the available services for accessing and using the data and functionality in an 
application.  
2.4 Implement and Monitor 
Activate the data services that have been developed and tested. Real-time data processing requires real-time 
monitoring for issues. Establish parameters that indicate potential problems with processing, as well as direct 
notification of issues. Automated as well as human monitoring for issues should be established, especially as the 
complexity and risk of the triggered responses rises. There are cases, for example, where issues with automated 
financial securities trading algorithms have triggered actions that have affected entire markets or bankrupted 
organizations. 
 

