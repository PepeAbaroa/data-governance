# página 469 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA QUALITY • 465 
•
Consistency rules: Conditional assertions that refer to maintaining a relationship between two (or
more) attributes based on the actual values of those attributes. For example, address validation where
postal codes correspond to particular States or Provinces.
•
Accuracy verification: Compare a data value against a corresponding value in a system of record or
other verified source (e.g., marketing data purchased from a vendor) to verify that the values match.
•
Uniqueness verification: Rules that specify which entities must have a unique representation and
whether one and only one record exists for each represented real world object.
•
Timeliness validation: Rules that indicate the characteristics associated with expectations for
accessibility and availability of data.
Other types of rules may involve aggregating functions applied to sets of data instances (see Section 4.5). 
Examples of aggregation checks include: 
•
Validate reasonableness of the number of records in a file. This requires keeping statistics over time to
generate trends.
•
Validate reasonableness of an average amount calculated from a set of transactions. This requires
establishing thresholds for comparison, and may be based on statistics over time.
•
Validate the expected variance in the count of transactions over a specified timeframe. This requires
keeping statistics over time and using them to establish thresholds.
1.3.8 Common Causes of Data Quality Issues 
Data quality issues can emerge at any point in the data lifecycle, from creation to disposal. When investigating 
root causes, analysts should look for potential culprits, like problems with data entry, data processing, system 
design, and manual intervention in automated processes. Many issues will have multiple causes and 
contributing factors (especially if people have created ways to work around them). These causes of issues also 
imply ways to prevent issues: through improvement to interface design, testing of data quality rules as part of 
processing, a focus on data quality within system design, and strict controls on manual intervention in 
automated processes.  
1.3.8.1 Issues Caused by Lack of Leadership 
Many people assume that most data quality issues are caused by data entry errors. A more sophisticated 
understanding recognizes that gaps in or poor execution of business and technical processes cause many more 
problems than mis-keying. However, common sense says and research indicates that many data quality 
problems are caused by a lack of organizational commitment to high quality data, which itself stems from a lack 
of leadership, in the form of both governance and management.  
 

