# página 254 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

250 • DMBOK2 
multiple versions of the ‘truth’. To avoid data integrity issues, manage user identity data and role-group 
membership centrally. This is a requirement for the quality of data used for effective access control. Security 
administrators create, modify, and delete user accounts and role groups. Changes made to the group taxonomy 
and membership should receive appropriate approval. Changes should be tracked via a change management 
system. 
Applying data security measures inconsistently or improperly within an organization can lead to employee 
dissatisfaction and significant risk to the organization. Role-based security depends on clearly defined, 
consistently assigned roles.  
There are two ways to define and organize roles: as a grid (starting from the data), or in a hierarchy (starting 
from the user). 
2.3.3.1 Role Assignment Grid 
A grid can be useful for mapping out access roles for data, based on data confidentiality, regulations, and user 
functions. The Public User role can have access to all data ranked for General Audiences and not subject to any 
regulations. A Marketing role may have access to some PII information for use in developing campaigns, but 
not to any restricted data, or Client Confidential data. Table 14 shows a very simplified example. 
Table 14 Role Assignment Grid Example 
Confidentiality Level 
General Audience 
Client Confidential 
Restricted Confidential 
Not Regulated 
Public User Role 
Client Manager Role 
Restricted Access Role 
PII 
Marketing Role 
Client Marketing Role 
HR Role 
PCI 
Financial Role 
Client Financial Role 
Restricted Financial Role 
2.3.3.2 Role Assignment Hierarchy 
Construct group definitions at a workgroup or business unit level. Organize these roles in a hierarchy, so that 
child roles further restrict the privileges of parent roles. The ongoing maintenance of these hierarchies is a 
complex operation requiring reporting systems capable of granular drill down to individual user privileges. A 
security role hierarchy example is shown in Figure 65. 
2.3.4 Assess Current Security Risks 
Security risks include elements that can compromise a network and/or database. The first step in identifying risk 
is identifying where sensitive data is stored, and what protections are required for that data. Evaluate each 
system for the following: 
 

