# página 243 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA SECURITY • 239 
system such as MS-Excel. Using MS-Excel and his legitimate login credentials, the worker might retrieve and 
save all patient records.  
There are two risks to consider: intentional and unintentional abuse. Intentional abuse occurs when an employee 
deliberately misuses organizational data. For example, an errant worker who wants to trade patient records for 
money or for intentional damage, such as releasing (or threatening to release) sensitive information publicly. 
Unintentional abuse is a more common risk: The diligent employee who retrieves and stores large amounts of 
patient information to a work machine for what he or she considers legitimate work purposes. Once the data 
exists on an endpoint machine, it becomes vulnerable to laptop theft and loss.  
The partial solution to the abuse of legitimate privilege is database access control that not only applies to 
specific queries, but also enforces policies for end-point machines using time of day, location monitoring, and 
amount of information downloaded, and reduces the ability of any user to have unlimited access to all records 
containing sensitive information unless it is specifically demanded by their job and approved by their 
supervisor. For example while it may be necessary for a field agent to access their customer’s personal records, 
they might not be allowed to download the entire customer database to their laptop just to ‘save time’. 
1.3.13.3 Unauthorized Privilege Elevation 
Attackers may take advantage of database platform software vulnerabilities to convert access privileges from 
those of an ordinary user to those of an administrator. Vulnerabilities may occur in stored procedures, built-in 
functions, protocol implementations, and even SQL statements. For example, a software developer at a financial 
institution might take advantage of a vulnerable function to gain the database administrative privilege. With 
administrative privilege, the offending developer may turn off audit mechanisms, create bogus accounts, 
transfer funds, or close accounts. 
Prevent privilege elevation exploits with a combination of traditional intrusion prevention systems (IPS) and 
query-level access control intrusion prevention. These systems inspect database traffic to identify patterns that 
correspond to known vulnerabilities. For example, if a given function is vulnerable to an attack, an IPS may 
either block all access to the procedure, or block those procedures allowing embedded attacks.  
Combine IPS with alternative attack indicators, such as query access control, to improve accuracy in identifying 
attacks. IPS can detect whether a database request accesses a vulnerable function while query access control 
detects whether the request matches normal user behavior. If a single request indicates both access to a 
vulnerable function and unusual behavior, then an attack is almost certainly occurring. 
1.3.13.4 Service Account or Shared Account Abuse 
Use of service accounts (batch IDs) and shared accounts (generic IDs) increases the risk of data security 
breaches and complicates the ability to trace the breach to its source. Some organizations further increase their 
 

