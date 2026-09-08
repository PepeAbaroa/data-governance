# página 466 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

462 • DMBOK2 
the exchange of encoded data.81 ISO 22745 creates portable data by labeling the data using an ISO 22745 
compliant Open Technical Dictionary such as the ECCMA Open Technical Dictionary (eOTD). 
The intention of ISO 8000 is to help organizations define what is and is not quality data, enable them to ask for 
quality data using standard conventions, and verify that they have received quality data using those same 
standards. When standards are followed, requirements can be confirmed through a computer program.  
ISO 8000 - Part 61 Information and data quality management process reference model is under development.82 
This standard will describe the structure and organization of data quality management, including: 
•
Data Quality Planning
•
Data Quality Control
•
Data Quality Assurance
•
Data Quality Improvement
1.3.6 Data Quality Improvement Lifecycle 
Most approaches to improving data quality are based on the techniques of quality improvement in the 
manufacture of physical products.83 In this paradigm, data is understood as the product of a set of processes. At 
its simplest, a process is defined as a series of steps that turns inputs into outputs. A process that creates data 
may consist of one-step (data collection) or many steps: data collection, integration into a data warehouse, 
aggregation in a data mart, etc. At any step, data can be negatively affected. It can be collected incorrectly, 
dropped or duplicated between systems, aligned or aggregated incorrectly, etc. Improving data quality requires 
the ability to assess the relationship between inputs and outputs, in order to ensure that inputs meet the 
requirements of the process and that outputs conform to expectations. Since outputs from one process become 
inputs to other processes, requirements must be defined along the whole data chain.  
A general approach to data quality improvement, shown in Figure 93, is a version of the Shewhart / Deming 
cycle.84 Based on the scientific method, the Shewhart / Deming cycle is a problem-solving model known as 
‘plan-do-check-act’. Improvement comes through a defined set of steps. The condition of data must be 
measured against standards and, if it does not meet standards, root cause(s) of the discrepancy from standards 
must be identified and remediated. Root causes may be found in any of the steps of the process, technical or 
non-technical. Once remediated, data should be monitored to ensure that it continues to meet requirements.  
81 http://bit.ly/2rUZyoz. 
82 http://bit.ly/2sVik3Q. 
83 See Wang (1998), English (1999), Redman (2001), Loshin (2001), and McGilvray (2008). See Pierce (2004) for an 
overview of literature related to the concept of data as a product. 
84 See American Society for Quality: http://bit.ly/1lelyBK Plan-Do-Check-Act was originated by Walter Shewhart and 
popularized by W. Edwards Deming. 6 Sigma’s Measure, Analyze, Improve, Control (DMAIC) is a variation on this cycle.  
 

