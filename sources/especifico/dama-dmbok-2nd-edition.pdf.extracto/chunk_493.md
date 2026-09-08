# página 494 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

490 • DMBOK2 
measurements to detect unexpected variation as soon as it is detectable. Early detection of problems simplifies 
investigation of their root causes. Measurements of the process can also be used to reduce the unwanted effects 
of common causes of variation, allowing for increased efficiency. 
4.6 Root Cause Analysis 
A root cause of a problem is a factor that, if eliminated, would remove the problem itself. Root cause analysis is 
a process of understanding factors that contribute to problems and the ways they contribute. Its purpose is to 
identify underlying conditions that, if eliminated, would mean problems would disappear.  
A data management example may clarify the definition. Let’s say a data process that runs each month requires 
as input a file of customer information. Measurement of the data shows that in April, July, October, and 
January, the quality of the data goes down. Inspection of the timing of delivery shows that in March, June, 
September, and December, the file is delivered on the 30th of the month, whereas at other times it is delivered on 
the 25th. Further analysis shows that the team responsible for delivering the file is also responsible for closing 
quarterly financial processes. These processes take precedence over other work and the files are delivered late 
during those months, impacting the quality. The root cause of the data quality problem turns out to be a process 
delay caused by a competing priority. It can be addressed by scheduling file delivery and ensuring that 
resources can deliver within the schedule.  
Common techniques for root cause analysis include Pareto analysis (the 80/20 rule), fishbone diagram analysis, 
track and trace, process analysis, and the Five Whys (McGilvray, 2008). 
5. Implementation Guidelines
Improving the quality of data within an organization is not an easy task – even when data quality improvement 
efforts are launched from within a data governance program and with the support of senior management. A 
classic academic discussion is whether it is better to implement a Data Quality program top-down or bottom-up. 
Typically, a hybrid approach works best – top-down for sponsorship, consistency, and resources, but bottom-up 
to discover what is actually broken and to achieve incremental successes. 
Improving data quality requires changes in how people think about and behave toward data. Cultural change is 
challenging. It requires planning, training, and reinforcement. (See Chapter 17.) While the specifics of cultural 
change will differ from organization to organization, most Data Quality program implementations need to plan 
for: 
•
Metrics on the value of data and the cost of poor quality data: One way to raise organizational
awareness of the need for Data Quality Management is through metrics that describe the value of data
and the return on investment from improvements. These metrics (which differ from data quality
scores) provide the basis for funding improvements and changing the behavior of both staff and
management. (See Chapter 11.)
 

