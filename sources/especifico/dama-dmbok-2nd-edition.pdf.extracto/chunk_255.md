# página 256 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

252 • DMBOK2 
Document the requirements for allowing original user authorizations so de-authorization may happen when 
these conditions no longer apply.  
For instance, a policy to ‘maintain appropriate user privileges’ could have a control objective of ‘Review DBA 
and User rights and privileges on a monthly basis’. The organization’s procedure to satisfy this control might 
be to implement and maintain processes to:  
•
Validate assigned permissions against a change management system used for tracking all user
permission requests
•
Require a workflow approval process or signed paper form to record and document each change
request
•
Include a procedure for eliminating authorizations for people whose job status or department no longer
qualifies them to have certain access rights
Some level of management must formally request, track, and approve all initial authorizations and subsequent 
changes to user and group authorizations 
2.3.5.1 Assign Confidentiality Levels 
Data Stewards are responsible for evaluating and determining the appropriate confidentiality level for data 
based on the organization’s classification scheme.  
The classification for documents and reports should be based on the highest level of confidentiality for any 
information found within the document. (See Chapter 9.) Label each page or screen with the classification in the 
header or footer. Information products classified as least confidential (e.g., “For General Audiences”) do not 
need labels. Assume any unlabeled products to be for General Audiences.  
Document authors and information product designers are responsible for evaluating, correctly classifying, and 
labeling the appropriate confidentiality level for each document, as well as each database, including relational 
tables, columns, and user entitlement views. 
In larger organizations, much of the security classification and protective effort will be the responsibility of a 
dedicated information security organization. While Information Security will be happy to have the Data 
Stewards work with these classifications, they usually take responsibility for enforcement and for physically 
protecting the network. 
2.3.5.2 Assign Regulatory Categories 
Organizations should create or adopt a classification approach to ensure that they can meet the demands of 
regulatory compliance. (See Section 3.3.) This classification scheme provides a foundation for responding to 
internal and external audits. Once it is in place, information needs to be assessed and classified within the 
schema. Security staff may not be familiar with this concept, as they do not work with individual data 
 

