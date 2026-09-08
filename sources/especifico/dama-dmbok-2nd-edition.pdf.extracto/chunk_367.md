# página 368 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

364 • DMBOK2 
1.3.3.4.4.2 Identity Resolution 
Some matches occur with great confidence, based on exact data matches across multiple fields. Other matches 
are suggested with less confidence due to conflicting values. For example: 
•
If two records share the same last name, first name, birth date, and social security number, but the
street address differs, is it safe to assume they refer to the same person who has changed their mailing
address?
•
If two records share the same social security number, street address, and first name, but the last name
differs, is it safe to assume they refer to the same person who has changed their last name? Would the
likelihood be increased or decreased based on gender and age?
•
How do these examples change if the social security number is unknown for one record? What other
identifiers are useful to determine the likelihood of a match? How much confidence is required for the
organization to assert a match?
Table 26 illustrates the conclusion of the process for the sample records in Table 24 and Table 25. Here the 
second two entity instances (Source ID 234 and 345) are determined to represent the same person (Jane Smith), 
while the first one (Source ID 123) is identified as representing a different person (John Smith).  
Table 26 Candidate Identification and Identity Resolution 
Source 
ID 
Name 
Address (Cleansed) 
Telephone 
(Cleansed) 
Candidate ID 
Party ID 
123 
John Smith 
123 Main, Dataland, SQ 98765 
 
XYZ 
1 
234 
J. Smith 
123 Main, Dataland, SQ 98765 
+1 234 567 8900 
XYZ, ABC 
2 
345 
Jane Smith 
123 Main, Dataland, SQ 98765 
+1 234 567 8900 
ABC 
2 
Despite the best efforts, match decisions sometimes prove to be incorrect. It is essential to maintain the history 
of matches so that matches can be undone when discovered to be incorrect. Match rate metrics enable 
organizations to monitor the impact and effectiveness of their matching inference rules. Reprocessing of match 
rules can help identify better match candidates as new information is received by the entity resolution process. 
1.3.3.4.4.3 Matching Workflows / Reconciliation Types 
Match rules for different scenarios require different workflows: 
•
Duplicate identification match rules focus on a specific set of data elements that uniquely identify an
entity and identify merge opportunities without taking automatic action. Business Data Stewards can
review these occurrences and decide to take action on a case-by-case basis.
•
Match-link rules identify and cross-reference records that appear to relate to a master record without
updating the content of the cross-referenced record. Match-link rules are easier to implement and much
easier to reverse.
 

