# página 479 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA QUALITY • 475 
Having identified the critical data, Data Quality analysts need to identify business rules that describe or imply 
expectations about the quality characteristics of data. Often rules themselves are not explicitly documented. 
They may need to be reverse-engineered through analysis of existing business processes, workflows, 
regulations, policies, standards, system edits, software code, triggers and procedures, status code assignment 
and use, and plain old common sense. For example, if a marketing company wants to target efforts at people in 
a specific demographic, then potential indexes of data quality might be the level and reasonability of population 
in demographic fields like birth date, age, gender, and household income.  
Most business rules are associated with how data is collected or created, but data quality measurement centers 
around whether data is fit for use. The two (data creation and data use) are related. People want to use data 
because of what it represents and why it was created. For example, to understand an organization’s sales 
performance during a specific quarter or over time depends on having reliable data about the sales process 
(number and type of units sold, volume sold to existing customers vs. new customers, etc.). 
It is not possible to know all the ways that data might be used, but it is possible to understand the process and 
rules by which data was created or collected. Measurements that describe whether data is fit for use should be 
developed in relation to known uses and measurable rules based on dimensions of data quality: completeness, 
conformity, validity, integrity, etc. that provide the basis for meaningful metrics. Dimensions of quality enable 
analysts to characterize both rules (field X is mandatory and must be populated) and findings (e.g., the field is 
not populated in 3% of the records; the data is only 97% complete). 
At the field or column level, rules can be straightforward. Completeness rules are a reflection of whether a field 
is mandatory or optional, and, if optional, the conditions under which it should be populated. Validity rules are 
dependent on stipulating the domain of valid values and, in some cases, the relationship between fields. For 
example, a US ZIP Code needs to be valid, in and of itself, and correctly associated with a US State code. Rules 
should also be defined at the data set level. For example, every customer must have a valid mailing address.  
Defining data quality rules is challenging because most people are not used to thinking about data in terms of 
rules. It may be necessary to get at the rules indirectly, by asking stakeholders about the input and output 
requirements of a business process. It also helps to ask about pain points, what happens when data is missing or 
incorrect, how they identify issues, how they recognize bad data, etc. Keep in mind that it is not necessary to 
know all the rules in order to assess data. Discovery and refinement of rules is an ongoing process. One of the 
best ways to get at rules is to share results of assessments. These results often give stakeholders a new 
perspective on the data from which they can articulate rules that tell them what they need to know about the 
data.  
2.4 Perform an Initial Data Quality Assessment 
Once the most critical business needs and the data that supports them have been identified, the most important 
part of the data quality assessment is actually looking at that data, querying it to understand data content and 
relationships, and comparing actual data to rules and expectations. The first time this is done, analysts will 
discover many things: undocumented relationships and dependencies within the data, implied rules, redundant 
 

