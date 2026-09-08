# página 358 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

354 • DMBOK2 
cases, it is better to maintain distinct lists that are related vs. attempting to have a single list that is the standard 
for all user communities. Table 18 provides an example related to status codes for help desk tickets. Without the 
information provided by the definition, ticket status would be ambiguous to anyone unfamiliar with the system. 
This differentiation is especially necessary for classifications driving performance metrics or other Business 
Intelligence analytics.  
Table 18 Simple Reference List Expanded 
Code 
Description 
Definition 
1 
New 
Indicates a newly created ticket without an assigned resource 
2 
Assigned 
Indicates a ticket that has a named resource assigned 
3 
Work In Progress 
Indicates the assigned resource started working on the ticket 
4 
Resolved 
Indicates request is assumed to be fulfilled per the assigned resource 
5 
Cancelled 
Indicates request was cancelled based on requester interaction 
6 
Pending 
Indicates request cannot proceed without additional information 
7 
Fulfilled 
Indicates request was fulfilled and verified by the requester 
1.3.2.1.2 Cross-Reference Lists 
Different applications may use different code sets to represent the same concept. These code sets may be at 
different granularities or the same granularity with different values. Cross-reference data sets translate between 
codes values. Table 19 presents a US State Code cross-reference (an example of multiple representations at the 
same level of grain). The US Postal Service State Codes are two character alpha codes. FIPS uses a numeric to 
express the same concept. The ISO State Code also includes a reference to the country.  
Table 19 Cross-Reference List 
USPS 
State 
Code 
ISO State 
Code 
FIPS 
Numeric 
State Code 
State 
Abbreviation 
State 
Name 
Formal State Name 
CA 
US-CA 
06 
Calif. 
California 
State of California 
KY 
US-KY 
21 
Ky. 
Kentucky 
Commonwealth of Kentucky 
WI 
US-WI 
55 
Wis. 
Wisconsin 
State of Wisconsin 
Language requirements may affect Reference Data structure. Multi-language lists are a specific instance of a 
cross-reference list. While code lists provide a standard, machine-readable format, language-specific glossaries 
provide usable content. Table 20 provides an example from the ISO 3166 standard. There are different ways to 
handle multi-language lists depending on how many languages and character sets are involved. Lists do not 
need to be normalized to be effective. The denormalized structure makes it somewhat easier to comprehend the 
relationships. 
Table 20 Multi-Language Reference List 
ISO 3166-1 Alpha 2 
Country Code 
English Name 
Local Name 
Local Name  
Local Alphabet 
French 
Name 
… 
CN 
China 
Zhong Guo 
中国/中國 
Chine 
 

