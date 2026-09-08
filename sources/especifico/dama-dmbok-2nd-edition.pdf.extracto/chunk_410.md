# página 411 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA WAREHOUSING AND BUSINESS INTELLIGENCE • 407 
•
Drill down / up: Drilling down or up is a specific analytical technique whereby the user navigates
among levels of data, ranging from the most summarized (up) to the most detailed (down).
•
Roll-up: A roll-up involves computing all of the data relationships for one or more dimensions. To do
this, define a computational relationship or formula.
•
Pivot: A pivot changes the dimensional orientation of a report or page display.
Three classic implementation approaches support Online Analytical Processing. 
•
Relational Online Analytical Processing (ROLAP): ROLAP supports OLAP by using techniques
that implement multi-dimensionality in the two-dimensional tables of relational database management
systems (RDBMS). Star schema joins are a common database design technique used in ROLAP
environments.
•
Multi-dimensional Online Analytical Processing (MOLAP): MOLAP supports OLAP by using
proprietary and specialized multi-dimensional database technology.
•
Hybrid Online Analytical Processing (HOLAP): This is simply a combination of ROLAP and
MOLAP. HOLAP implementations allow part of the data to be stored in MOLAP form and another
part of the data to be stored in ROLAP. Implementations vary on the control a designer has to vary the
mix of partitioning.
4. Techniques
4.1 Prototypes to Drive Requirements 
Quickly prioritize requirements before the implementation activities begin by creating a demonstration set of 
data and applying discovery steps in a joint prototype effort. Advances in data virtualization technologies can 
alleviate some of the traditional implementation pains through collaborative prototyping techniques. 
Profiling the data contributes to prototyping and helps reduces risk associated with unexpected data. The DW is 
often the first place where the pain of poor quality data in source systems or data entry functions becomes 
apparent. Profiling also discloses differences between sources that may present obstacles to data integration. 
Data may be of high quality within its sources, but because sources, differ the data integration process becomes 
more complicated.  
Evaluation of the state of the source data leads to more accurate up-front estimates for feasibility and scope of 
effort. The evaluation is also important for setting appropriate expectations. Plan to collaborate with the Data 
Quality and Data Governance team(s) and to draw on the expertise of other SMEs to understand data 
discrepancies and risks. (See Chapters 11 and 13.)  
 

