# página 443 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

METADATA MANAGEMENT • 439 
2.4.1 Integrate Metadata 
Integration processes gather and consolidate Metadata from across the enterprise, including Metadata from data 
acquired outside the enterprise. The Metadata repository should integrate extracted technical Metadata with 
relevant business, processes, and stewardship Metadata. Metadata can be extracted using adapters, scanners, 
bridge applications, or by directly accessing the Metadata in a source data store. Adapters are available with 
many third party vendor software tools, as well as from Metadata integration tools. In some cases, adapters will 
be developed using the tool API’s.  
Challenges arise in integration that will require governance. Integrating internal data sets, external data such as 
government statistics, and data sourced from non-electronic forms, such as white papers, articles in magazines, 
or reports, can raise numerous questions on quality and semantics. 
Accomplish repository scanning in two distinct approaches. 
•
Proprietary interface: In a single-step scan and load process, a scanner collects the Metadata from a
source system, then directly calls the format-specific loader component to load the Metadata into the
repository. In this process, there is no format-specific file output and the collection and loading of
Metadata occurs in a single step.
•
Semi-proprietary interface: In a two-step process, a scanner collects the Metadata from a source
system and outputs it into a format-specific data file. The scanner only produces a data file that the
receiving repository needs to be able to read and load appropriately. The interface is a more open
architecture, as the file is readable by many methods.
A scanning process uses and produces several types of files during the process. 
•
Control file: Containing the source structure of the data model
•
Reuse file: Containing the rules for managing reuse of process loads
•
Log files: Produced during each phase of the process, one for each scan or extract and one for each
load cycle
•
Temporary and backup files: Use during the process or for traceability
Use a non-persistent Metadata staging area to store temporary and backup files. The staging area supports 
rollback and recovery processes, and provides an interim audit trail to assist repository managers when 
investigating Metadata source or quality issues. The staging area may take the form of a directory of files or a 
database.  
Data Integration tools used for data warehousing and Business Intelligence applications are often used 
effectively in Metadata integration processes. (See Chapter 8.) 
2.4.2 Distribute and Deliver Metadata 
Metadata is delivered to data consumers and to applications or tools that require Metadata feeds. Delivery 
mechanisms include: 
 

