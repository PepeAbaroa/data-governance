# página 257 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA SECURITY • 253 
regulations, but with infrastructure systems. They will need to have documented requirements for data 
protection relating to these categories defining actions they can implement. 
2.3.5.3 Manage and Maintain Data Security 
Once all the requirements, policies, and procedures are in place, the main task is to ensure that security breaches 
do not occur, and if they do, to detect them as soon as possible. Continual monitoring of systems and auditing of 
the execution of security procedures are crucial to preserving data security.  
2.3.5.3.1 Control Data Availability / Data-centric Security 
Controlling data availability requires management of user entitlements and of the structures (data masking, view 
creation, etc.) that technically control access based on entitlements. Some databases are better than others in 
providing structures and processes to protect data in storage. (See Section 3.7.)  
Security Compliance managers may have direct responsibility for designing user entitlement profiles that allow 
the business to function smoothly, while following relevant restrictions. 
Defining entitlements and granting authorizations requires an inventory of data, careful analysis of data needs, 
and documentation of the data exposed in each user entitlement. Often highly sensitive information is mixed 
with non-sensitive information. An enterprise data model is essential to identifying and locating sensitive data. 
(See Section 1.1.1.) 
Data masking can protect data even if it is inadvertently exposed. Certain data regulations require encryption, an 
extreme version of in-place masking. Authorization to the decryption keys can be part of the user authorization 
process. Users authorized to access the decryption keys can see the unencrypted data, while others only see 
random characters. 
Relational database views can used to enforce data security levels. Views can restrict access to certain rows 
based on data values or restrict access to certain columns, limiting access to confidential or regulated fields. 
2.3.5.3.2 Monitor User Authentication and Access Behavior 
Reporting on access is a basic requirement for compliance audits. Monitoring authentication and access 
behavior provides information about who is connecting and accessing information assets. Monitoring also helps 
detect unusual, unforeseen, or suspicious transactions that warrant investigation. In this way, it compensates for 
gaps in data security planning, design, and implementation. 
Deciding what needs monitoring, for how long, and what actions to take in the event of an alert, requires careful 
analysis driven by business and regulatory requirements. Monitoring entails a wide range of activities. It can be 
specific to certain data sets, users, or roles. It can be used to validate data integrity, configurations, or core 
 

