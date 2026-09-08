# página 468 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

464 • DMBOK2 
The cost of getting data right the first time is cheaper than the costs from getting data wrong and fixing it later. 
Building quality into the data management processes from the beginning costs less than retrofitting it. 
Maintaining high quality data throughout the data lifecycle is less risky than trying to improve quality in an 
existing process. It also creates a far lower impact on the organization. Establishing criteria for data quality at 
the beginning of a process or system build is one sign of a mature Data Management Organization. Doing so 
takes governance and discipline, as well as cross-functional collaboration. 
1.3.7 Data Quality Business Rule Types 
Business rules describe how business should operate internally, in order to be successful and compliant with the 
outside world. Data Quality Business Rules describe how data should exist in order to be useful and usable 
within an organization. These rules can be aligned with dimensions of quality and used to describe data quality 
requirements. For example, a business rule that all state code fields must comply with the US State 
Abbreviations can be enforced by data entry pick lists and data integration lookups. The level of valid or invalid 
records can then be measured.  
Business rules are commonly implemented in software, or by using document templates for data entry. Some 
common simple business rule types are: 
•
Definitional conformance: Confirm that the same understanding of data definitions is implemented
and used properly in processes across the organization. Confirmation includes algorithmic agreement
on calculated fields, including any time, or local constraints, and rollup and status interdependence
rules.
•
Value presence and record completeness: Rules defining the conditions under which missing values
are acceptable or unacceptable.
•
Format compliance: One or more patterns specify values assigned to a data element, such as
standards for formatting telephone numbers.
•
Value domain membership: Specify that a data element’s assigned value is included in those
enumerated in a defined data value domain, such as 2-Character United States Postal Codes for a
STATE field.
•
Range conformance: A data element assigned value must be within a defined numeric, lexicographic,
or time range, such as greater than 0 and less than 100 for a numeric range.
•
Mapping conformance: Indicating that the value assigned to a data element must correspond to one
selected from a value domain that maps to other equivalent corresponding value domain(s). The
STATE data domain again provides a good example, since State values may be represented using
different value domains (USPS Postal codes, FIPS 2-digit codes, full names), and these types of rules
validate that ‘AL’ and ‘01’ both map to ‘Alabama.’
 

