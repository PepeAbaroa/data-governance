# página 233 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA SECURITY • 229 
•
Randomization: Replace part or all of data elements with either random characters or a series of a
single character.
•
Encryption: Convert a recognizably meaningful character stream to an unrecognizable character
stream by means of a cipher code. An extreme version of obfuscation in-place.
•
Expression masking: Change all values to the result of an expression. For example, a simple
expression would just hard code all values in a large free form database field (that could potentially
contain confidential data) to be ‘This is a comment field’.
•
Key masking: Designate that the result of the masking algorithm/process must be unique and
repeatable because it is being used mask a database key field (or similar). This type of masking is
extremely important for testing to maintain integrity around the organization.
1.3.10 Network Security Terms 
Data security includes both data-at-rest and data-in-motion. Data-in-motion requires a network in order to move 
between systems. It is no longer sufficient for an organization to wholly trust in the firewall to protect it from 
malicious software, poisoned email, or social engineering attacks. Each machine on the network needs to have a 
line of defense, and web servers need sophisticated protection as they are continually exposed to the entire 
world on the Internet.  
1.3.10.1 Backdoor 
A backdoor refers to an overlooked or hidden entry into a computer system or application. It allows 
unauthorized users to bypass the password requirement to gain access. Backdoors are often created by 
developers for maintenance purposes. Any backdoor is a security risk. Other backdoors are put in place by the 
creators of commercial software packages.  
Default passwords left unchanged when installing any software system or web page package is a backdoor and 
will undoubtedly be known to hackers. Any backdoor is a security risk. 
1.3.10.2 Bot or Zombie 
A bot (short for robot) or Zombie is a workstation that has been taken over by a malicious hacker using a 
Trojan, a Virus, a Phish, or a download of an infected file. Remotely controlled, bots are used to perform 
malicious tasks, such as sending large amounts of spam, attacking legitimate businesses with network-clogging 
 

