# página 493 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA QUALITY • 489 
median, or mode) and of variability around a central value (e.g., range, variance, standard deviation), to 
establish tolerances for variation within a process.  
The primary tool used for SPC is the control chart (Figure 95), which is a time series graph that includes a 
central line for the average (the measure of central tendency) and depicts calculated upper and lower control 
limits (variability around a central value). In a stable process, measurement results outside the control limits 
indicate a special cause.  
Figure 95 Control Chart of a Process in Statistical Control 
SPC measures the predictability of process outcomes by identifying variation within a process. Processes have 
variation of two types: Common Causes that are inherent in the process and Special Causes that are 
unpredictable or intermittent. When the only sources of variation are common causes, a system is said to be in 
(statistical) control and a range of normal variation can be established. This is the baseline against which change 
can be detected.  
Applying SPC to data quality measurement is based on the working assumption that, like a manufactured 
product, data is the product of a process. Sometimes the process that creates data is very simple (e.g., a person 
fills out a form). Other times, processes are quite complex: a set of algorithms aggregates medical claim data in 
order to follow trends related to the effectiveness of particular clinical protocols. If such a process has consistent 
inputs and is executed consistently, it will produce consistent results each time it is run. However, if the inputs 
or execution change, then so will the outputs. Each of these components can be measured. The measurements 
can be used to detect special causes. Knowledge of the special causes can be used to mitigate risks associated 
with data collection or processing.  
SPC is used for control, detection, and improvement. The first step is to measure the process in order to identify 
and eliminate special causes. This activity establishes the control state of the process. Next is to put in place 
0,17
0,18
0,19
0,20
0,21
Percentage of defaults per load
Example of Data from a Stable (in-control) Process
UCL=0,21061
͞x=0.1885
LCL=0,16639
TGT_TBL_ETL_DT
0,16
 

[1 imágenes en esta página]
