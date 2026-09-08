# página 244 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

240 • DMBOK2 
risk when they configure monitoring systems to ignore any alerts related to these accounts. Information security 
managers should consider adopting tools to manage service accounts securely.  
1.3.13.4.1 Service Accounts 
Service accounts are convenient because they can tailor enhanced access for the processes that use them. 
However, if they are used for other purposes, they are untraceable to a particular user or administrator. Unless 
they have access to decryption keys, service accounts do not threaten encrypted data. This may be especially 
important for data held on servers storing legal documents, medical information, trade secrets, or confidential 
executive planning. 
Restrict the use of service accounts to specific tasks or commands on specific systems, and require 
documentation and approval for distributing the credentials. Consider assigning a new password every time 
distribution occurs, using processes such as those in place for Super User accounts. 
1.3.13.4.2 Shared Accounts 
Shared accounts are created when an application cannot handle the number of user accounts needed or when 
adding specific users requires a large effort or incurs additional licensing costs. For shared accounts, credentials 
are given to multiple users, and the password is rarely changed due to the effort to notify all users. Because they 
provide essentially ungoverned access, any use of shared accounts should be carefully evaluated. They should 
never be used by default. 
1.3.13.5 Platform Intrusion Attacks 
Software updates and intrusion prevention protection of database assets requires a combination of regular 
software updates (patches) and the implementation of a dedicated Intrusion Prevention Systems (IPS). An IPS is 
usually, but not always, implemented alongside of an Intrusion Detection System (IDS). The goal is to prevent 
the vast majority of network intrusion attempts and to respond quickly to any intrusion that has succeeded in 
working its way past a prevention system. The most primitive form of intrusion protection is a firewall, but with 
mobile users, web access, and mobile computing equipment a part of most enterprise environments, a simple 
firewall, while still necessary, is no longer sufficient. 
Vendor-provided updates reduce vulnerabilities found in database platforms over time. Unfortunately, software 
updates are often implemented by enterprises according to periodic maintenance cycles rather than as soon as 
possible after the patches are made available. In between update cycles, databases are not protected. In addition, 
compatibility problems sometimes prevent software updates altogether. To address these problems, implement 
IPS.  
 

