# página 476 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

472 • DMBOK2 
•
Psychographic information: Data used to segment the target populations by specific behaviors,
habits, or preferences, such as product and brand preferences, organization memberships, leisure
activities, commuting transportation style, shopping time preferences, etc.
•
Valuation information: Use this kind of enhancement for asset valuation, inventory, and sale.
1.3.10.3 Data Parsing and Formatting 
Data Parsing is the process of analyzing data using pre-determined rules to define its content or value. Data 
parsing enables the data analyst to define sets of patterns that feed into a rule engine used to distinguish between 
valid and invalid data values. Matching specific pattern(s) triggers actions.  
Data parsing assigns characteristics to the data values appearing in a data instance, and those characteristics 
help in determining potential sources for added benefits. For example, if an attribute called ‘name’ can be 
determined to have values belonging to ‘business name’ embedded within it, then the data value is identified as 
the name of a business rather than the name of a person. Use the same approach for any situation in which data 
values organize into semantic hierarchies such as sub-parts, parts, and assemblies. 
Many data quality issues involve situations where variation in data values representing similar concepts 
introduces ambiguity. Extract and rearrange the separate components (commonly referred to as ‘tokens’) can be 
extracted and rearranged into a standard representation to create a valid pattern. When an invalid pattern is 
recognized, the application may attempt to transform the invalid value into one that meets the rules. Perform 
standardization by mapping data from some source pattern into a corresponding target representation. 
For example, consider the different ways telephone numbers expected to conform to a numbering plan are 
formatted. While some have digits, some have alphabetic characters, and all use different special characters for 
separation. People can recognize each one as a telephone number. However, to determine if these numbers are 
accurate (perhaps by comparing them to a master customer directory), or to investigate whether duplicate 
numbers exist when there should be only one for each supplier, the values must be parsed into their component 
segments (area code, exchange, and line number) and then transformed into a standard format.  
Another good example is a customer name, since names may be represented in thousands of different forms. A 
good standardization tool will be able to parse the different components of a customer name, such as given 
name, middle name, family name, initials, titles, generational designations, and then rearrange those 
components into a canonical representation that other data services will be able to manipulate. 
The human ability to recognize familiar patterns contributes to an ability to characterize variant data values 
belonging to the same abstract class of values; people recognize different types of telephone numbers because 
they conform to frequently used patterns. An analyst describes the format patterns that all represent a data 
object, such as Person Name, Product Description, and so on. A data quality tool parses data values that 
conform to any of those patterns, and even transforms them into a single, standardized form that will simplify 
the assessment, similarity analysis, and remediation processes. Pattern-based parsing can automate the 
recognition and subsequent standardization of meaningful value components. 
 

