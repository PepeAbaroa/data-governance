# página 357 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

REFERENCE AND MASTER DATA • 353 
•
Reference Data Management systems that maintain business entities, allowed, future-state, or
deprecated values, and term mapping rules to support broader application and data integration use
•
Object attribute specific Metadata to specify permissible values with a focus on API or user interface
access
Reference Data Management entails control and maintenance of defined domain values, definitions, and the 
relationships within and across domain values. The goal of Reference Data Management is to ensure values are 
consistent and current across different functions and that the data is accessible to the organization. Like other 
data, Reference Data requires Metadata. An important Metadata attribute for Reference Data includes its source. 
For example, the governing body for industry standard Reference Data.  
1.3.2.1 Reference Data Structure 
Depending on the granularity and complexity of what the Reference Data represents, it may be structured as a 
simple list, a cross-reference, or a taxonomy. The ability to use and maintain Reference Data should be 
accounted for when structuring it within a database or a Reference Data Management system.  
1.3.2.1.1 Lists 
The simplest form of Reference Data pairs a code value with a description in a list, such as in Table 17. The 
code value is the primary identifier, the short form reference value that appears in other contexts. The 
description states what the code represents. The description may be displayed in place of the code on screens, 
pages, drop-down lists, and reports. Note that in this example, the code value for United Kingdom is GB 
according to international standards, and not UK, even though UK is a common short form used in many forms 
of communication. Balance between standards compliance and usability when defining Reference Data 
requirements.  
Table 17 Simple Reference List 
Code Value 
Description 
US 
United States of America 
GB 
United Kingdom (Great Britain) 
Depending on the content and complexity of the Reference Data, additional attributes may be required to define 
the meaning of the code. Definitions provide information that the label alone does not provide. Definitions 
rarely appear on reports or drop-down lists. However, they do appear in places like Help functions for 
applications, which guide the appropriate use of codes in context.  
Lists, like any Reference Data, must meet the requirements of data consumers, including requirements for the 
appropriate level of detail. If a list of values is intended to support data classification by casual users, a highly 
detailed list will likely cause data quality issues and adoption challenges. Similarly, a list of values that is too 
generic would prevent knowledge workers from capturing sufficient level of detail. To accommodate such 
 

