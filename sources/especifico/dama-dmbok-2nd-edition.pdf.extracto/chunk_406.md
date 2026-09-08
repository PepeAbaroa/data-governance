# página 407 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA WAREHOUSING AND BUSINESS INTELLIGENCE • 403 
•
Investigation of the root causes of data issues
•
Impact analysis for system changes or data issues
•
Ability to determine the reliability of data, based on its origin
Look to implement an integrated impact and lineage tool that can understand all the moving parts involved in 
the load process, as well as end user reporting and analytics. Impact analysis reports will outline which 
components are affected by a potential change, expediting and streamlining estimating and maintenance tasks.  
Many key business processes, relationships, and terminologies are captured and explained during development 
of the data model. The logical data model holds much of this information, which is often lost or ignored during 
development or production deployment. It is critical to ensure that this information is not discarded and that the 
logical and physical models are updated after deployment and are in sync.  
3.2 Data Integration Tools 
Data integration tools are used to populate a data warehouse. In addition to doing the work of integrating data, 
they enable scheduling of jobs in ways that account for complex data delivery from multiple sources. In 
selecting a tool, also account for these features that enable management of the system: 
•
Process audit, control, restart, and scheduling
•
The ability to selectively extract data elements at execution time and pass that extract to a downstream
system for audit purposes
•
Controlling which operations can or cannot execute and restarting a failed or aborted run (see Chapter
8)
A variety of data integration tools also offer integration capabilities with the BI portfolio, supporting import and 
export of workflow messages, email, or even semantic layers. Workflow integration can drive data quality 
defect identification, resolution, and escalation processes. Messaging through email or alert processing driven 
from email is a common practice especially for mobile devices. In addition, the ability to provision a data target 
as a semantic layer can be a data virtualization candidate for agile implementations. 
3.3 Business Intelligence Tools Types 
The maturity of the BI market, and a wide range of available BI tools, makes it rare for companies to build their 
own BI tools.68 The purpose of this section is to introduce the types of tools available in the BI marketplace, and 
provide an overview of their chief characteristics with information to help match the tools to the appropriate 
68 The material in this section is primarily from “The Business Intelligence Market” by Cindi Howson, BIScorecard®, 
http://bit.ly/2tNirv5; used by permission, with minor changes and additions. 
 

