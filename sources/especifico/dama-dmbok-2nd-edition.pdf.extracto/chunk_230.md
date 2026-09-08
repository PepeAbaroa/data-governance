# página 231 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA SECURITY • 227 
1.3.8.1 Hash 
Hash encryption uses algorithms to convert data into a mathematical representation. The exact algorithms used 
and order of application must be known in order to reverse the encryption process and reveal the original data. 
Sometimes hashing is used as verification of transmission integrity or identity. Common hashing algorithms are 
Message Digest 5 (MD5) and Secure Hashing Algorithm (SHA). 
1.3.8.2 Private-key 
Private-key encryption uses one key to encrypt the data. Both the sender and the recipient must have the key to 
read the original data. Data can be encrypted one character at a time (as in a stream) or in blocks. Common 
private-key algorithms include Data Encryption Standard (DES), Triple DES (3DES), Advanced Encryption 
Standard (AES), and International Data Encryption Algorithm (IDEA). Cyphers Twofish and Serpent are also 
considered secure. The use of simple DES is unwise as it is susceptible to many easy attacks. 
1.3.8.3 Public-key 
In public-key encryption, the sender and the receiver have different keys. The sender uses a public key that is 
freely available, and the receiver uses a private key to reveal the original data. This type of encryption is useful 
when many data sources must send protected information to just a few recipients, such as when submitting data 
to clearinghouses. Public-key methods include Rivest-Shamir-Adelman (RSA) Key Exchange and Diffie-
Hellman Key Agreement. PGP (Pretty Good Privacy) is a freely available application of public-key encryption. 
1.3.9 Obfuscation or Masking 
Data can be made less available by obfuscation (making obscure or unclear) or masking, which removes, 
shuffles, or otherwise changes the appearance of the data, without losing the meaning of the data or the 
relationships the data has to other data sets, such as foreign key relationships to other objects or systems. The 
values within the attributes may change, but the new values are still valid for those attributes. Obfuscation is 
useful when displaying sensitive information on screens for reference, or creating test data sets from production 
data that comply with expected application logic.  
Data masking is a type of data-centric security. There are two types of data masking, persistent and dynamic. 
Persistent masking can be executed in-flight or in-place. 
1.3.9.1 Persistent Data Masking 
Persistent data masking permanently and irreversibly alters the data. This type of masking is not typically used 
in production environments, but rather between a production environment and development or test 
 

