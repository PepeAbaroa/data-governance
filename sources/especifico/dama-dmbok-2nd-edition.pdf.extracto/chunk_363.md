# página 364 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

360 • DMBOK2 
Master Data Management is challenging. It illustrates a fundamental challenge with data: People choose 
different ways to represent similar concepts and reconciliation between these representations is not always 
straightforward; as importantly, information changes over time and systematically accounting for these changes 
takes planning, data knowledge, and technical skills. In short, it takes work.  
Any organization that has recognized the need for MDM probably already has a complex system landscape, 
with multiple ways of capturing and storing references to real world entities. Because of both organic growth 
over time or from mergers and acquisitions, the systems that provided input to the MDM process may have 
different definitions of the entities themselves and very likely have different standards for Data Quality. 
Because of this complexity, it is best to approach Master Data Management one data domain at a time. Start 
small, with a handful of attributes, and build out over time.  
Planning for Master Data Management includes several basic steps. Within a domain: 
•
Identify candidate sources that will provide a comprehensive view of the Master Data entities
•
Develop rules for accurately matching and merging entity instances
•
Establish an approach to identify and restore inappropriately matched and merged data
•
Establish an approach to distribute trusted data to systems across the enterprise
Executing the process, though, is not as simple as these steps imply, as MDM is a lifecycle management 
process. Activities critical to the lifecycle include: 
•
Establishing the context of Master Data entities, including definitions of associated attributes and the
conditions of their use. This process requires governance.
•
Identifying multiple instances of the same entity represented within and across data sources; building
and maintaining identifiers and cross-references to enable information integration.
•
Reconciling and consolidating data across sources to provide a master record or the best version of the
truth. Consolidated records provide a merged view of information across systems and seek to address
attribute naming and data value inconsistencies.
•
Identifying improperly matched or merged instances and ensuring they are resolved and correctly
associated with identifiers.
•
Provisioning of access to trusted data across applications, either through direct reads, data services, or
by replication feeds to transactional, warehousing or analytical data stores.
•
Enforcing the use of Master Data values within the organization. This process also requires governance
and change management to assure a shared enterprise perspective.
1.3.3.4 Master Data Management Key Processing Steps 
Key processing steps for MDM are illustrated in Figure 76. They include data model management; data 
acquisition; data validation, standardization, and enrichment; entity resolution; and stewardship and sharing. 
In a comprehensive MDM environment, the logical data model will be physically instantiated in multiple 
platforms. It guides the implementation of the MDM solution, providing the basis of data integration services. It 
 

