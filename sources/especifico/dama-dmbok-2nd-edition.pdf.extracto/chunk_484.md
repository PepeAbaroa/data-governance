# página 485 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA QUALITY • 481 
Provide continuous monitoring by incorporating control and measurement processes into the information 
processing flow. Automated monitoring of conformance to data quality rules can be done in-stream or through a 
batch process. Measurements can be taken at three levels of granularity: the data element value, data instance or 
record, or the data set. Table 31 describes techniques for collecting data quality measurements. In-stream 
measurements can be taken while creating data or handing data off between processing stages. Batch queries 
can be performed on collections of data instances assembled in a data set, usually in persistent storage. Data set 
measurements generally cannot be taken in-stream, since the measurement may need the entire set.  
Incorporating the results of the control and measurement processes into both the operational procedures and 
reporting frameworks enables continuous monitoring of the levels of data quality for feedback and improvement 
to the data generation/collection activities. 
Table 31 Data Quality Monitoring Techniques 
Granularity 
In-stream (In-Process Flow) Treatment 
Batch Treatment 
Data Element 
Edit checks in application 
Data element validation services 
Specially programmed applications 
Direct queries 
Data profiling or analyzer tool 
Data Record 
Edit checks in application 
Data record validation services 
Specially programmed applications 
Direct queries 
Data profiling or analyzer tool 
Data set 
Inspection inserted between processing stages 
Direct queries 
Data profiling or analyzer tool 
2.7.3 Develop Operational Procedures for Managing Data Issues 
Whatever tools are used to monitor data quality, when results are assessed by Data Quality team members, they 
need to respond to findings in a timely and effective manner. The team must design and implement detailed 
operational procedures for: 
•
Diagnosing issues: The objective is to review the symptoms of the data quality incident, trace the
lineage of the data in question, identify the problem and where it originated, and pinpoint potential root
causes of the problem. The procedure should describe how the Data Quality Operations team would:
o
Review the data issues in the context of the appropriate information processing flows and
isolate the location in the process where the flaw is introduced
o
Evaluate whether there have been any environmental changes that would cause errors entering
into the system
o
Evaluate whether or not there are any other process issues that contributed to the data quality
incident
o
Determine whether there are issues with external data that have affected the quality of the data
NOTE: The work of root cause analysis requires input from technical and business SMEs. While the 
DQ team may lead and facilitate this kind of work effort, success requires cross-functional 
collaboration  
 

