# página 239 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA SECURITY • 235 
•
Regulation: Regulatory categories are assigned based on external rules, such as laws, treaties, customs
agreements, and industry regulations. Regulatory information is shared on an ‘allowed-to-know’ basis.
The ways in which data can be shared are governed by the details of the regulation.
The main difference between confidential and regulatory restrictions is where the restriction originates: 
confidentiality restrictions originate internally, while regulatory restrictions are externally defined.  
Another difference is that any data set, such as a document or a database view, can only have one 
confidentiality level. This level is established based on the most sensitive (and highest classified) item in the 
data set. Regulatory categorizations, however, are additive. A single data set may have data restricted based on 
multiple regulatory categories. To assure regulatory compliance, enforce all actions required for each category, 
along with the confidentiality requirements.  
When applied to the user entitlement (the aggregation of the particular data elements to which a user 
authorization provides access), all protection policies must be followed, regardless of whether they originated 
internally or externally. 
1.3.12.1 Confidential Data 
Confidentiality requirements range from high (very few people have access, for example, to data about 
employee compensation) to low (everyone has access to product catalogs). A typical classification schema 
might include two or more of the five confidentiality classification levels listed here: 
•
For general audiences: Information available to anyone, including the public.
•
Internal use only: Information limited to employees or members, but with minimal risk if shared. For
internal use only; may be shown or discussed, but not copied, outside the organization.
•
Confidential: Information that cannot be shared outside the organization without a properly executed
non-disclosure agreement or similar in place. Client confidential information may not be shared with
other clients.
•
Restricted confidential: Information limited to individuals performing certain roles with the ‘need to
know.’ Restricted confidential may require individuals to qualify through clearance.
•
Registered confidential: Information so confidential that anyone accessing the information must sign
a legal agreement to access the data and assume responsibility for its secrecy.
The confidentiality level does not imply any details about restrictions due to regulatory requirements. For 
example, it does not inform the data manager that data may not be exposed outside its country of origin, or that 
some employees are prohibited from seeing certain information based on regulations like HIPAA.  
 

