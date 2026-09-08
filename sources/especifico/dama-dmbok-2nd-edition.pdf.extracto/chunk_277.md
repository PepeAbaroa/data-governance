# página 278 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

274 • DMBOK2 
•
Semantic conversion: Conversion of data values to maintain consistent semantic representation. For
example, the source gender codes might include 0, 1, 2, and 3, while the target gender codes might be
represented as UNKNOWN, FEMALE, MALE, or NOT PROVIDED.
•
De-duping: Ensuring that if rules require unique key values or records, a means for scanning the
target, and detecting and removing duplicate rows, is included
•
Re-ordering: Changing the order of the data elements or records to fit a defined pattern
Transformation may be performed in batch or real-time, either physically storing the result in a staging area, or 
virtually storing the transformed data in memory until ready to move to the load step. Data resulting from the 
transformation stage should be ready to integrate with data in the target structure.  
1.3.1.3 Load 
The load step of ETL is physically storing or presenting the result of the transformations in the target system. 
Depending on the transformations performed, the target system’s purpose, and the intended use, the data may 
need further processing to be integrated with other data, or it may be in a final form, ready to present to 
consumers. 
Figure 67 ETL Process Flow 
1.3.1.4 ELT 
If the target system has more transformation capability than either the source or an intermediary application 
system, the order of processes may be switched to ELT – Extract, Load, and Transform. ELT allows 
Transform
Process
Load
Process
Lookups
Mappings
Extract
Process
Source
Datastore
Staging
Datastore
Target
Datastore
 

[14 imágenes en esta página]
