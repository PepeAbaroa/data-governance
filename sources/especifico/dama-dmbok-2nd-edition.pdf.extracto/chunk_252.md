# página 253 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA SECURITY • 249 
require from the enterprise. Often the regulations imply a goal, and it is up to the corporation to determine the 
means for reaching that information protection goal. Actions that can be audited provide legal proof of 
compliance. 
A useful way to handle the data-specific regulations is by analyzing and grouping similar regulations into 
categories, as was been done by grouping various risks into a few security classifications.  
With more than one-hundred different data-specific ordinances around the world, it would be useless to develop 
a different category for each regulation. Most data regulations, imposed as they are by separate legal entities, 
seek to do the same thing. For example, the contractual obligations for protecting confidential customer data are 
remarkably similar to U.S., Japanese, and Canadian government regulations for protecting Personally 
Identifiable Information, and similar for compliance with EU privacy requirements. This pattern is easy to see 
when the auditable compliance actions for each regulation are listed and compared. Thus, they may all be 
managed properly by using the same protective action category.  
A key principle for both security classification and regulatory categorization is that most information can be 
aggregated so that it has greater or lesser sensitivity. Developers need to know how aggregations affect the 
overall security classification and regulatory categories. When a developer of a dashboard, report, or database 
view knows that some of the data that is required may be personally private or insider or related to competitive 
advantage, the system can then be designed to eliminate aspects of that from the entitlement, or, if the data must 
remain in the user-entitlement, to enforce all the security and regulatory requirements at the time of user 
authorization.  
The results of this classification work will be a formally approved set of security classifications and regulatory 
categories and a process for capturing this Metadata in a central repository so that employees, both business and 
technical, know the sensitivity if the information they are handling, transmitting, and authorizing 
2.3.3 Define Security Roles 
Data access control can be organized at an individual or group level, depending on the need. That said, granting 
access and update privileges to individual user accounts entails a great deal of redundant effort. Smaller 
organizations may find it acceptable to manage data access at the individual level. However, larger 
organizations will benefit greatly from role-based access control, granting permissions to role groups and 
thereby to each group member.  
Role groups enable security administrators to define privileges by role and to grant these privileges by enrolling 
users in the appropriate role group. While it is technically possible to enroll a user in more than one group, this 
practice may make it difficult to understand the privileges granted to a specific user. Whenever possible, try to 
assign each user to only one role group. This may require the creation of different user views of certain data 
entitlements to comply with regulations. 
Data consistency in user and role management is a challenge. User information such as name, title, and 
employee ID must be stored redundantly in several locations. These islands of data often conflict, representing 
 

