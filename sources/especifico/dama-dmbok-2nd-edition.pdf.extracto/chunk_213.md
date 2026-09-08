# página 214 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

210 • DMBOK2 
4. Techniques
4.1 Test in Lower Environments 
For upgrades and patches to operating systems, database software, database changes, and code changes, install 
and test on the lowest level environment first – usually development. Once tested on the lowest level, install on 
the next higher levels, and install on the production environment last. This ensures that the installers have 
experience with the upgrade or patch, and can minimize disruption to the production environments. 
4.2 Physical Naming Standards 
Consistency in naming speeds understanding. Data architects, database developers, and DBAs can use naming 
standards for defining Metadata or creating rules for exchanging documents between organizations. 
ISO/IEC 11179 – Metadata registries (MDR), addresses the semantics of data, the representation of data, and 
the registration of the descriptions of that data. It is through these descriptions that an accurate understanding of 
the semantics and a useful depiction of the data are found. 
The significant section for physical databases within that standards is Part 5 – Naming and Identification 
Principles, which describes how to form conventions for naming data elements and their components. 
4.3 Script Usage for All Changes 
It is extremely risky to directly change data in a database. However, there may be a need, such as an annual 
change in the chart of accounts structures, or in mergers and acquisitions, or emergencies, where these are 
indicated due to the ‘one-off’ nature of the request and/or the lack of appropriate tools for these circumstances. 
It is helpful to place changes to be made into update script files and test them thoroughly in non-production 
environments before applying to production. 
5. Implementation Guidelines
5.1 Readiness Assessment / Risk Assessment  
A risk and readiness assessment revolves around two central ideas: risk of data loss and risks related to 
technology readiness. 
 

