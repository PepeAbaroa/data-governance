# página 406 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

402 • DMBOK2 
3. Tools
Choosing the initial set of tools can be a long process. It includes attempting to satisfy near-term requirements, 
non-functional specifications, and the as-yet to be created next generation requirements. Decision criteria tool 
sets, process implementation tools, and professional services offerings can facilitate and expedite this activity. It 
is critical to evaluate not only the conventional build or buy positions, but also the rent option provisioned as 
Software-as-a-Service. Renting SaaS tools and the associated expertise is weighed against the cost of building 
from scratch or deploying purchased products from vendors. Consider ongoing upgrade and potential 
replacement costs as well. Alignment to a set OLA (Operational Level Agreement) can bridge forecasted costs, 
and provide input into setting compelling fees and penalties for term violations.  
3.1 Metadata Repository 
Large organizations often find themselves with many tools from different vendors, each deployed potentially at 
differing versions. Key to this effort is the ability to stitch Metadata together from a variety of sources. 
Automating and integrating population of this repository can be achieved with a variety of techniques. (See 
Chapter 13.) 
3.1.1 Data Dictionary / Glossary 
A data dictionary is necessary to support the use of a DW. The dictionary describes data in business terms and 
includes other information needed to use the data (e.g., data types, details of structure, security restrictions). 
Often the content for the data dictionary comes directly from the logical data model. Plan for high quality 
Metadata by ensuring modelers take a disciplined approach to managing definitions as part of the modeling 
process.  
In some organizations, business users actively participate in the development of the data dictionary by 
supplying, defining, and then stewarding corrections to definitions of subject area data elements. Embrace this 
activity through a collaboration tool, monitor activities through a Center of Excellence, and ensure that content 
created through this activity is retained in the logical model. Ensuring agreement between the business-facing 
content and the technical-facing physical data model will reduce the risk of downstream errors and rework. (See 
Chapter 13.) 
3.1.2 Data and Data Model Lineage 
Many data integration tools offer lineage analysis that considers both the developed population code and the 
physical data model and database. Some offer web interfaces to monitor and update definitions and other 
Metadata. Documented data lineage serves many purposes:  
 

