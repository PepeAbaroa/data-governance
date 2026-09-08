# página 373 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

REFERENCE AND MASTER DATA • 369 
external organizations, a managed and reconciled version of the information is maintained in the organization’s 
own systems. 
Examples of licensed reference directories include Dun and Bradstreet’s (D&B) Company Directory of 
worldwide Company Headquarters, Subsidiaries, and Branch locations, and the American Medical 
Association’s Prescriber Database. 
Reference directories enable Master Data use by: 
•
Providing a starting point for matching and linking new records. For example, in an environment with
five data sources, each source can be compared against the directory (5 comparison points) vs. against
each other (10 comparison points).
•
Providing additional data elements that may not be as easily available at the time of record creation
(e.g., for a physician, this may include medical license status; for a company, this may include a six
digit NAICS industry classification).
As an organization’s records match and reconcile with the reference directories, the trusted record will deviate 
from the reference directory with traceability to other source records, contributing attributes, and transformation 
rules. 
1.3.4 Data Sharing Architecture 
There are several basic architectural approaches to reference and Master Data integration. Each Master Data 
subject area will likely have its own system of record. For example, the human resource system usually serves 
as the system of record for employee data. A CRM system might serve as the system of record for customer 
data, while an ERP system might serve as the system of record for financial and product data. 
The data sharing hub architecture model shown in Figure 77 represents a hub-and-spoke architecture for Master 
Data. The Master Data hub can handle interactions with spoke items such as source systems, business 
applications, and data stores while minimizing the number of integration points. A local data hub can extend 
and scale the Master Data hub. (See Chapter 8.) 
Each of the three basic approaches to implementing a Master Data hub environment has pros and cons: 
•
A Registry is an index that points to Master Data in the various systems of record. The systems of
record manage Master Data local to their applications. Access to Master Data comes from the master
index. A registry is relatively easy to implement because it requires few changes in the systems of
record. But often, complex queries are required to assemble Master Data from multiple systems.
Moreover, multiple business rules need to be implemented to address semantic differences across
systems in multiple places.
•
In a Transaction Hub, applications interface with the hub to access and update Master Data. The
Master Data exists within the Transaction Hub and not within any other applications. The Transaction
Hub is the system of record for Master Data. Transaction Hubs enable better governance and provide a
 

