# página 370 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

366 • DMBOK2 
Data architecture design of an MDM solution must resolve whether to leverage parent-child relationships, 
affiliation relationships, or both for a given entity.  
•
Affiliation relationships provide the greatest flexibility through programming logic. The relationships
type can be used to expose such data in a parent-child hierarchy. Many downstream solutions, such as
reporting or account navigation tools would want to see a hierarchical view of the information.
•
Parent-Child relationships require less programming logic as the navigation structure is implied.
However, if the relationship changes and there isn’t an available affiliation structure, this may
influence the quality of the data and Business Intelligence dimensions.
1.3.3.4.5 Data Sharing and Stewardship 
Although much of the work of Master Data Management can be automated through tools that enable processing 
of large numbers of records, it still requires stewardship to resolve situations where data is incorrectly matched. 
Ideally, lessons learned from the stewardship process can be used to improve matching algorithms and reduce 
instances of manual work. (See Chapters 3 and 8.)  
1.3.3.5 Party Master Data 
Party Master Data includes data about individuals, organizations, and the roles they play in business 
relationships. In the commercial environment, parties include customers, employees, vendors, partners, and 
competitors. In the public sector, parties are usually citizens. Law enforcement focuses on suspects, witnesses, 
and victims. Not-for-profit organizations focus on members and donors. While in healthcare, the focus is on 
patients and providers; in education, it is on students and faculty. 
Customer Relationship Management (CRM) systems manage Master Data about customers. The goal of CRM 
is to provide complete and accurate information about each and every customer.  
An essential aspect of CRM is identifying duplicate, redundant, or conflicting data from different systems and 
determining whether the data represents one or more than one customer. CRM must be able to resolve 
conflicting values, reconcile differences, and accurately represent current knowledge of the customer. This 
process requires robust rules as well as knowledge of the structure, granularity, lineage, and quality of data 
sources.  
Specialized MDM systems perform similar functions for individuals, organizations and their roles, employees, 
and vendors. Regardless of industry or focus, managing business party Master Data poses unique challenges: 
•
The complexity of roles and relationships played by individuals and organizations
•
Difficulties in unique identification
•
The number of data sources and the differences between them
•
The multiple mobile and social communications channels
 

