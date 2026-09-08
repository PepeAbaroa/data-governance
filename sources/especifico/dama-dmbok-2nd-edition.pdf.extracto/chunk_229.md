# página 230 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

226 • DMBOK2 
•
Authorization: Grant individuals privileges to access specific views of data, appropriate to their role.
After the authorization decision, the Access Control System checks each time a user logs in to see if
they have a valid authorization token. Technically, this is an entry in a data field in the corporate
Active Directory indicating that the person has been authorized by somebody to access the data. It
further indicates that a responsible person made the decision to grant this authorization because the
user is entitled to it by virtue of their job or corporate status.
•
Entitlement: An Entitlement is the sum total of all the data elements that are exposed to a user by a
single access authorization decision. A responsible manager must decide that a person is ‘entitled’ to
access this information before an authorization request is generated. An inventory of all the data
exposed by each entitlement is necessary in determining regulatory and confidentiality requirements
for Entitlement decisions.
1.3.6.2 Monitoring 
Systems should include monitoring controls that detect unexpected events, including potential security 
violations. Systems containing confidential information, such as salary or financial data, commonly implement 
active, real-time monitoring that alerts the security administrator to suspicious activity or inappropriate access.  
Some security systems will actively interrupt activities that do not follow specific access profiles. The account 
or activity remains locked until security support personnel evaluate the details.  
In contrast, passive monitoring tracks changes over time by taking snapshots of the system at regular intervals, 
and comparing trends against a benchmark or other criteria. The system sends reports to the data stewards or 
security administrator accountable for the data. While active monitoring is a detection mechanism, passive 
monitoring is an assessment mechanism. 
1.3.7 Data Integrity 
In security, data integrity is the state of being whole – protected from improper alteration, deletion, or addition. 
For example, in the U.S., Sarbanes-Oxley regulations are mostly concerned with protecting financial 
information integrity by identifying rules for how financial information can be created and edited.  
1.3.8 Encryption 
Encryption is the process of translating plain text into complex codes to hide privileged information, verify 
complete transmission, or verify the sender’s identity. Encrypted data cannot be read without the decryption key 
or algorithm, which is usually stored separately and cannot be calculated based on other data elements in the 
same data set. There are four main methods of encryption – hash, symmetric, private-key, and public-key – with 
varying levels of complexity and key structure. 
 

