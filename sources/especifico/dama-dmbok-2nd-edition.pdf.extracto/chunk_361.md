# página 362 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

358 • DMBOK2 
Master Data should represent the authoritative, most accurate data available about key business entities. When 
managed well, Master Data values are trusted and can be used with confidence.  
Business rules typically dictate the format and allowable ranges of Master Data values. Common organizational 
Master Data includes data about: 
•
Parties, made up of individuals and organizations, and their roles, such as customers, citizens, patients,
vendors, suppliers, agents, business partners, competitors, employees, or students
•
Products and Services, both internal and external
•
Financial structures, such as contracts, general ledger accounts, cost centers, or profit centers
•
Locations, such as addresses and GPS coordinates
1.3.3.1 System of Record, System of Reference 
When there are potentially different versions of ‘the truth’, it is necessary to distinguish between them. In order 
to do so, one must know where data originates or is accessed, and which data has been prepared for particular 
uses. A System of Record is an authoritative system where data is created/captured, and/or maintained through a 
defined set of rules and expectations (e.g., an ERP system may be the System of Record for sell-to customers). 
A System of Reference is an authoritative system where data consumers can obtain reliable data to support 
transactions and analysis, even if the information did not originate in the system of reference. MDM 
applications, Data Sharing Hubs, and Data Warehouses often serve as systems of reference.  
1.3.3.2 Trusted Source, Golden Record 
A Trusted Source is recognized as the ‘best version of the truth’ based on a combination of automated rules and 
manual stewardship of data content. A trusted source may also be referred to as a Single View, 360° View. Any 
MDM system should be managed so that it is a trusted source. Within a trusted source, records that represent 
the most accurate data about entity instances can be referred to as Golden Records.  
The term Golden Record can be misleading. Tech Target defines a Golden Record as “the ‘single version of the 
truth’, where ‘truth’ is understood to mean the reference to which data users can turn when they want to ensure 
that they have the correct version of a piece of information. The golden record encompasses all the data in every 
system of record (SOR) within a particular organization.”59  
However, the two parts of this definition bring the concept into question, as data in different systems may not 
align into ‘a single version of the truth’.  
Within any Master Data effort, the merging/resolution of data from multiple sources into a ‘Golden Record’ 
does not mean that it is always a 100% complete and 100% accurate representation of all the entities within the 
59 http://bit.ly/2rRJI3b. 
 

