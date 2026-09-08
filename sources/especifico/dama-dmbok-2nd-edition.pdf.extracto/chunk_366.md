# página 367 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

REFERENCE AND MASTER DATA • 363 
executing the process differ based on the approach they take to determining similarity between two references. 
While resolution always takes place between pairs of references, the process can be systematically extended to 
include large data sets. Entity resolution is critical to MDM, as the process of matching and merging records 
enables the construction of the Master Data set.  
Entity resolution includes a set of activities (reference extraction, reference preparation, reference resolution, 
identity management, relationship analysis) that enable the identity of entity instances and the relationship 
between entity instances, to be managed over time. Within the process of reference resolution, two references 
may be identified as representing the same entity, through the process of determining equivalency. These 
references can then be linked through a value (a global identifier) that indicates that they are equivalent 
(Talburt, 2011).  
1.3.3.4.4.1 Matching  
Matching, or candidate identification, is the process of identifying how different records may relate to a single 
entity. The risks with this process are: 
•
False positives: Two references that do not represent the same entity are linked with a single identifier.
This results in one identifier that refers to more than one real-world entity instance.
•
False negatives: Two references represent the same entity but they are not linked with a single
identifier. This results in multiple identifiers that refer to the same real-world entity when each instance
is expected to have one-and-only-one identifier.
Both situations are addressed through a process called similarity analysis or matching, in which the degree of 
similarity between any two records is scored, often based on weighted approximate matching between 
corresponding attribute values. If the score is above a specified threshold, the two records are considered to 
represent the same entity (a match). Through similarity analysis, slight variations in data can be recognized and 
data values can be consolidated. Two basic approaches, which can be used together, are deterministic and 
probabilistic:  
•
Deterministic algorithms, like parsing and standardization, rely on defined patterns and rules for
assigning weights and scores for determining similarity. Deterministic algorithms are predictable in
that the patterns matched and the rules applied will always yield the same results. This type of
matching works out-of-the-box with relatively good performance, but it is only as good as the
situations anticipated by the people who developed the rules.
•
Probabilistic algorithms rely on statistical techniques for assessing the probability that any pair of
records represents the same entity. This relies on the ability to take data samples for training purposes
by looking at the expected results for a subset of the records and tuning the matcher to self-adjust
based on statistical analysis. These matchers are not reliant on rules, so the results may be
nondeterministic. However, because the probabilities can be refined based on experience, probabilistic
matchers are able to improve their matching precision as more data is analyzed.
 

