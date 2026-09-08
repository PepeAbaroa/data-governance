# página 245 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA SECURITY • 241 
1.3.13.6 SQL Injection Vulnerability 
In a SQL injection attack, a perpetrator inserts (or ‘injects’) unauthorized database statements into a vulnerable 
SQL data channel, such as stored procedures and Web application input spaces. These injected SQL statements 
are passed to the database, where they are often executed as legitimate commands. Using SQL injection, 
attackers may gain unrestricted access to an entire database.  
SQL injections are also used to attack the DBMS, by passing SQL commands as a parameter of a function or 
stored procedure. For example, a component that provides backup functionality usually runs at a high privilege; 
calling a SQL injection vulnerable function in that specific component could allow a regular user to escalate 
their privileges, become a DBA and take over the database. 
Mitigate this risk by sanitizing all inputs before passing them back to the server. 
1.3.13.7 Default Passwords 
It is a long-standing practice in the software industry to create default accounts during the installation of 
software packages. Some are used in the installation itself. Others provide users with a means to test the 
software out of the box.  
Default passwords are part of many demo packages. Installation of third party software creates others. For 
example, a CRM package might create several accounts in the backend database, for install, test, and admin and 
for regular users. SAP creates a number of default database users at the time of installation. The DBMS industry 
also engages in this practice.  
Attackers are constantly looking for an easy way to steal sensitive data. Mitigate threats to sensitive data by 
creating the required username and password combinations, and ensuring the no default passwords are left in 
place in the DBMS. Eliminating the default passwords is an important security step after every implementation. 
1.3.13.8 Backup Data Abuse 
Backups are made to reduce the risks associated with data loss, but backups also represent a security risk. The 
news offers many stories about lost backup media. Encrypt all database backups. Encryption prevents loss of a 
backup either in tangible media or in electronic transit. Securely manage backup decryption keys. Keys must be 
available off-site to be useful for disaster recovery.  
1.3.14 Hacking / Hacker 
The term hacking came from an era when finding clever ways to perform some computer task was the goal. A 
hacker is a person who finds unknown operations and pathways within complex computer systems. Hackers can 
be good or bad.  
 

