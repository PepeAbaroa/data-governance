# página 302 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

298 • DMBOK2 
technical considerations in implementing business rules, a purely technical approach to DII can lead to errors in 
the data mappings and transformations as data flows into, through and out of an organization.  
Business stakeholders are responsible for defining rules for how data should be modeled and transformed. 
Business stakeholders should approve changes to any of these business rules. Rules should be captured as 
Metadata and consolidated for cross-enterprise analysis. Identifying and verifying the predictive models and 
defining what actions should be automatically triggered by the predictions are also business functions.  
Without trust that the integration or interoperable design will perform as promised, in a secure, reliable way, 
there can be no effective business value. In DII, the landscape of governance controls to support trust can be 
complex and detailed. One approach is to determine what events trigger governance reviews (exceptions or 
critical events). Map each trigger to reviews that engage with governance bodies. Event triggers may be part of 
the System Development Life Cycle (SDLC) at Stage Gates when moving from one phase to another or as part 
of User Stories. For example, architecture design compliance checklists may include such questions as: If 
possible, are you using the ESB and tools? Was there a search for reusable services?  
Controls may come from governance-driven management routines, such as mandated reviews of models, 
auditing of Metadata, gating of deliverables, and required approvals for changes to transformation rules.  
In Service Level Agreements, and in Business Continuity/Disaster Recovery plans, real-time operational data 
integration solutions must be included in the same backup and recovery tier as the most critical system to which 
they provide data. 
Policies need to be established to ensure that the organization benefits from an enterprise approach to DII. For 
example, policies can be put in place to ensure that SOA principles are followed, that new services are created 
only after a review of existing services, and that all data flowing between systems goes through the enterprise 
service bus.  
6.1 Data Sharing Agreements 
Prior to the development of interfaces or the provision of data electronically, develop a data sharing agreement 
or memorandum of understanding (MOU) which stipulates the responsibilities and acceptable use of data to be 
exchanged, approved by the business data stewards of the data in question. The data sharing agreements should 
specify anticipated use and access to the data, restrictions on use, as well as expected service levels, including 
required system up times and response times. These agreements are especially critical for regulated industries, 
or when personal or secure information is involved.  
6.2 DII and Data Lineage  
Data lineage is useful to the development of DII solutions. It is also often required for data consumers to use 
data, but it is becoming even more important as data is integrated between organizations. Governance is 
 

