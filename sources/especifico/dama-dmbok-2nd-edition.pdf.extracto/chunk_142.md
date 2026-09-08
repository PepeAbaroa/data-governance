# página 143 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 139 
1.3.4.2.1 Fact Tables 
Within a dimensional scheme, the rows of a fact table correspond to particular measurements and are numeric, 
such as amounts, quantities, or counts. Some measurements are the results of algorithms, in which case 
Metadata is critical to proper understanding and usage. Fact tables take up the most space in the database (90% 
is a reasonable rule of thumb), and tend to have large numbers of rows. 
1.3.4.2.2 Dimension Tables 
Dimension tables represent the important objects of the business and contain mostly textual descriptions. 
Dimensions serve as the primary source for ‘query by’ or ‘report by’ constraints, by acting as the entry points or 
links into the fact tables. Dimensions are typically highly denormalized and typically account for about 10% of 
the total data.  
Dimensions must have a unique identifier for each row. The two main approaches to identifying keys for 
dimension tables are surrogate keys and natural keys. 
Dimensions also have attributes that change at different rates. Slowly changing dimensions (SCDs) manage 
changes based on the rate and type of change. The three main types of change are sometimes known by ORC. 
•
Overwrite (Type 1): The new value overwrites the old value in place.
•
New Row (Type 2): The new values are written in a new row, and the old row is marked as not
current.
•
New Column (Type 3): Multiple instances of a value are listed in columns on the same row, and a
new value means writing the values in the series one spot down to make space at the front for the new
value. The last value is discarded.
1.3.4.2.3 Snowflaking 
Snowflaking is the term given to normalizing the flat, single-table, dimensional structure in a star schema into 
the respective component hierarchical or network structures.  
1.3.4.2.4 Grain 
The term grain stands for the meaning or description of a single row of data in a fact table; this is the most 
detail any row will have. Defining the grain of a fact table is one of the key steps in dimensional design. For 
example, if a dimensional model is measuring the student registration process, the grain may be student, day, 
and class.  
 

