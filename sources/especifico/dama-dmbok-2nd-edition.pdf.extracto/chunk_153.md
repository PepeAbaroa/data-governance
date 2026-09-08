# página 154 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

150 • DMBOK2 
•
Horizontally split: To reduce query sets, create subset tables using the value of a column as the
differentiator. For example, create regional customer tables that contain only customers in a specific
region.
1.3.5.3.4 Denormalization 
Denormalization is the deliberate transformation of normalized logical data model entities into physical tables 
with redundant or duplicate data structures. In other words, denormalization intentionally puts one attribute in 
multiple places. There are several reasons to denormalize data. The first is to improve performance by:  
•
Combining data from multiple other tables in advance to avoid costly run-time joins
•
Creating smaller, pre-filtered copies of data to reduce costly run-time calculations and/or table scans of
large tables
•
Pre-calculating and storing costly data calculations to avoid run-time system resource competition
Denormalization can also be used to enforce user security by segregating data into multiple views or copies of 
tables according to access needs. 
This process does introduce a risk of data errors due to duplication. Therefore, denormalization is frequently 
chosen if structures such as views and partitions fall short in producing an efficient physical design. It is good 
practice to implement data quality checks to ensure that the copies of the attributes are correctly stored. In 
general, denormalize only to improve database query performance or to facilitate enforcement of user security.  
Although the term denormalization is used in this section, the process does not apply just to relational data 
models. For example, one can denormalize in a document database, but it would be called something different – 
such as embedding.  
In dimensional data modeling, denormalization is called collapsing or combining. If each dimension is 
collapsed into a single structure, the resulting data model is called a Star Schema (see Figure 51). If the 
dimensions are not collapsed, the resulting data model is called a Snowflake (See Figure 49). 
1.3.6 Normalization 
Normalization is the process of applying rules in order to organize business complexity into stable data 
structures. The basic goal of normalization is to keep each attribute in only one place to eliminate redundancy 
and the inconsistencies that can result from redundancy. The process requires a deep understanding of each 
attribute and each attribute’s relationship to its primary key. 
Normalization rules sort attributes according to primary and foreign keys. Normalization rules sort into levels, 
with each level applying granularity and specificity in search of the correct primary and foreign keys. Each level 
 

