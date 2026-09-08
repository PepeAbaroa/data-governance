# página 184 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

180 • DMBOK2 
BASE-type systems are common in Big Data environments. Large online organizations and social media 
companies commonly use BASE implementations, as immediate accuracy of all data elements at all times is not 
necessary. Table 12 summarizes the differences between ACID and BASE.  
Table 12 ACID vs BASE 
Item 
ACID 
BASE 
Casting (data structure) 
Schema must exist 
Dynamic 
Table structure exists 
Adjust on the fly 
Columns data typed 
Store dissimilar data 
Consistency 
Strong Consistency Available 
Strong, Eventual, or None 
Processing Focus 
Transactional 
Key-value stores 
Processing Focus 
Row/Column 
Wide-column stores 
History 
1970s application storage 
2000s unstructured storage 
Scaling 
Product Dependent 
Automatically spreads data across 
commodity servers  
Origin 
Mixture 
Open-source 
Transaction 
Yes 
Possible 
1.3.5.3 CAP 
The CAP Theorem (or Brewer’s Theorem) was developed in response to a shift toward more distributed 
systems (Brewer, 2000). The theorem asserts that a distributed system cannot comply with all parts of ACID at 
all time. The larger the system, the lower the compliance. A distributed system must instead trade-off between 
properties.  
•
Consistency: The system must operate as designed and expected at all times.
•
Availability: The system must be available when requested and must respond to each request.
•
Partition Tolerance: The system must be able to continue operations during occasions of data loss or
partial system failure.
The CAP Theorem states that at most two of the three properties can exist in any shared-data system. This is 
usually stated with a ‘pick two’ statement, illustrated in Figure 58. 
Figure 58 CAP Theorem 
Partition Tolerance
No System Failures
CAP Theorem
“Pick Two”
CAP Theorem
“Pick Two”
CAP Theorem
“Pick Two”
Partition Tolerance
 

