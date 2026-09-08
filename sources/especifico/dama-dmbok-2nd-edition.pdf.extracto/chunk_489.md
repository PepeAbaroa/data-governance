# página 490 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

486 • DMBOK2 
4. Techniques
4.1 Preventive Actions 
The best way to create high quality data is to prevent poor quality data from entering an organization. 
Preventive actions stop known errors from occurring. Inspecting data after it is in production will not improve 
its quality. Approaches include:  
•
Establish data entry controls: Create data entry rules that prevent invalid or inaccurate data from
entering a system.
•
Train data producers: Ensure staff in upstream systems understand the impact of their data on
downstream users. Give incentives or base evaluations on data accuracy and completeness, rather than
just speed.
•
Define and enforce rules: Create a ‘data firewall,’ which has a table with all the business data quality
rules used to check if the quality of data is good, before being used in an application such a data
warehouse. A data firewall can inspect the level of quality of data processed by an application, and if
the level of quality is below acceptable levels, analysts can be informed about the problem.
•
Demand high quality data from data suppliers: Examine an external data provider’s processes to
check their structures, definitions, and data source(s) and data provenance. Doing so enables
assessment of how well their data will integrate and helps prevent the use of non-authoritative data or
data acquired without permission from the owner.
•
Implement Data Governance and Stewardship: Ensure roles and responsibilities are defined that
describe and enforce rules of engagement, decision rights, and accountabilities for effective
management of data and information assets (McGilvray, 2008). Work with data stewards to revise the
process of, and mechanisms for, generating, sending, and receiving data.
•
Institute formal change control: Ensure all changes to stored data are defined and tested before being
implemented. Prevent changes directly to data outside of normal processing by establishing gating
processes.
4.2 Corrective Actions 
Corrective actions are implemented after a problem has occurred and been detected. Data quality issues should 
be addressed systemically and at their root causes to minimize the costs and risks of corrective actions. ‘Solve 
the problem where it happens’ is the best practice in Data Quality Management. This generally means that 
corrective actions should include preventing recurrence of the causes of the quality problems.  
Perform data correction in three general ways: 
 

