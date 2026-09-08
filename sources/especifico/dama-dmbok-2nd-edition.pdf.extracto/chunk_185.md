# página 186 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

182 • DMBOK2 
using compression – where the state (for example) is stored as a pointer to a table of states, compressing the 
master table significantly.  
1.3.6.4 Flash Memory 
Recent advances in memory storage have made flash memory or solid state drives (SSDs) an attractive 
alternative to disks. Flash memory combines the access speed of memory-based storage with the persistence of 
disk-based storage.  
1.3.7 Database Environments 
Databases are used in a variety of environments during the systems development lifecycle. When testing 
changes, DBAs should be involved in designing the data structures in the Development environment. The DBA 
team should implement any changes to the QA environment, and must be the only team implementing changes 
to the Production environment. Production changes must adhere strictly to standard processes and procedures. 
While most data technology is software running on general purpose hardware, occasionally specialized 
hardware is used to support unique data management requirements. Types of specialized hardware include data 
appliances – servers built specifically for data transformation and distribution. These servers integrate with 
existing infrastructure either directly as a plug-in, or peripherally as a network connection. 
1.3.7.1 Production Environment 
The production environment is the technical environment where all business processes occur. Production is 
mission-critical – if this environment ceases to operate, business processes will stop, resulting in bottom-line 
losses, as well as a negative impact on customers who are unable to access services. In an emergency, or for 
public service systems, unexpected loss of function can be disastrous.  
The production environment is the ‘real’ environment from a business perspective. However, in order to have a 
reliable production environment, other non-production environments must exist and be used appropriately. For 
example, production environments should not be used for development and testing as these activities put 
production processes and data at risk. 
1.3.7.2 Pre-production Environments 
Pre-production environments are used to develop and test changes before such changes are introduced to the 
production environment. In pre-production environments, issues with changes can be detected and addressed 
without affecting normal business processes. In order to detect potential issues, the configuration of pre-
production environments must closely resemble the production environment.  
 

