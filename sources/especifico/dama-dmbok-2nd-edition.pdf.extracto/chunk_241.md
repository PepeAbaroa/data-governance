# página 242 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

238 • DMBOK2 
1.3.13 System Security Risks 
The first step in identifying risk is identifying where sensitive data is stored, and what protections are required 
for that data. It is also necessary to identify risks inherent in systems. System security risks include elements 
that can compromise a network or database. These threats allow legitimate employees to misuse information, 
either intentionally or accidentally, and enable malicious hacker success. 
1.3.13.1 Abuse of Excessive Privilege 
In granting access to data, the principle of least privilege should be applied. A user, process, or program should 
be allowed to access only the information allowed by its legitimate purpose. The risk is that users with 
privileges that exceed the requirements of their job function may abuse these privileges for malicious purpose or 
accidentally. Users may be granted more access than they should have (excessive privilege) simply because it is 
challenging to manage user entitlements. The DBA may not have the time or Metadata to define and update 
granular access privilege control mechanisms for each user entitlement. As a result, many users receive generic 
default access privileges that far exceed specific job requirements. This lack of oversight to user entitlements is 
one reason why many data regulations specify data management security.  
The solution to excessive privileges is query-level access control, a mechanism that restricts database privileges 
to minimum-required SQL operations and data. The granularity of data access control must extend beyond the 
table to specific rows and columns within a table. Query-level access control is useful for detecting excessive 
privilege abuse by malicious employees. 
Most database software implementations integrate some level of query-level access control (triggers, row-level 
security, table security, views), but the manual nature of these ‘built-in’ features make them impractical for all 
but the most limited deployments. The process of manually defining a query-level access control policy for all 
users across database rows, columns, and operations is time consuming. To make matters worse, as user roles 
change over time, query policies must be updated to reflect those new roles. Most database administrators 
would have a hard time defining a useful query policy for a handful of users at a single point in time, much less 
hundreds of users over time. As a result, in a large number of organizations, automated tools are usually 
necessary to make real query-level access control functional. 
1.3.13.2 Abuse of Legitimate Privilege 
Users may abuse legitimate database privileges for unauthorized purposes. Consider a criminally inclined 
healthcare worker with privileges to view individual patient records via a custom Web application.  
The structure of corporate Web applications normally limits users to viewing an individual patient’s healthcare 
history, where multiple records cannot be viewed simultaneously and electronic copies are not allowed. 
However, the worker may circumvent these limitations by connecting to the database using an alternative 
 

