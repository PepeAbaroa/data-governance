# página 300 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

296 • DMBOK2 
3.7 Metadata Repository 
A Metadata repository contains information about the data in an organization, including data structure, content, 
and the business rules for managing the data. During data integration projects, one or more Metadata 
repositories may be used to document the technical structure and business meaning of the data being sourced, 
transformed, and targeted.  
Usually the rules regarding data transformation, lineage, and processing used by the data integration tools are 
also stored in a Metadata repository as are the instructions for scheduled processes such as triggers and 
frequency. 
Every tool usually has its own Metadata repository. Suites of tools from the same vendor may share a Metadata 
repository. One Metadata repository may be designated as a central point for consolidating data from the 
various operational tools. (See Chapter 12.) 
4. Techniques
Several of the important techniques for designing data integration solutions are described in the Essential 
Concepts in this chapter. The basic goals are to keep the applications coupled loosely, limit the number of 
interfaces developed and requiring management by using a hub-and-spoke approach, and to create standard (or 
canonical) interfaces. 
5. Implementation Guidelines
5.1 Readiness Assessment / Risk Assessment 
All organizations have some form of DII already in place – so the readiness/risk assessment should be around 
enterprise integration tool implementation, or enhancing capabilities to allow interoperability. 
Implementing enterprise data integration solutions is usually cost-justified based on implementation between 
many systems. Design an enterprise data integration solution to support the movement of data between many 
applications and organizations, and not just the first one to be implemented.  
Many organizations spend their time reworking existing solutions instead of bringing additional value. Focus on 
implementing data integration solutions where none or limited integration currently exists, rather than replacing 
working data integration solutions with a common enterprise solution across the organization.  
 

