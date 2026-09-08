# página 262 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

258 • DMBOK2 
the largest number of data loss incidents result from the lack of sensitive data protection due to ignorance of its 
sensitivity, Metadata documentation completely overshadows any hypothetical risk that might occur if the 
Metadata were to be somehow exposed from the Metadata repository. This risk is made more negligible since it 
is trivial for an experienced hacker to locate unprotected sensitive data on the network. The people most likely 
unaware of the need to protect sensitive data appear to be employees and managers. 
3.7 Data Masking/Encryption 
Tools that perform masking or encryption are useful for restricting movement of sensitive data. (See Section 
1.3.9.) 
4. Techniques
Techniques for managing information security depend on the size of the organization, the architecture of the 
network, the type of data that must be secured, and the policies and standards used by a security organization.  
4.1 CRUD Matrix Usage 
Creating and using data-to-process and data-to-role relationship (CRUD–Create, Read, Update, Delete) matrices 
help map data access needs and guide definition of data security role groups, parameters, and permissions. 
Some versions add an E for Execute to make CRUDE. 
4.2 Immediate Security Patch Deployment 
A process for installing security patches as quickly as possible on all machines should be in place. A malicious 
hacker only needs root access to one machine in order to conduct his attack successfully on the network. Users 
should not be able to delay this update. 
4.3 Data Security Attributes in Metadata 
A Metadata repository is essential to assure the integrity and consistent use of an Enterprise Data Model across 
business processes. Metadata should include security and regulatory classifications for data. (See Section 1.1.3.) 
Having security Metadata in place protects an organization from employees who may not recognize the data as 
sensitive. When Data Stewards apply confidentiality and regulatory categories, category information should be 
documented in the Metadata repository and, if technology allows, tagged to the data. (See Sections 3.3.1 and 
 

