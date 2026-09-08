# página 296 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

292 • DMBOK2 
Developing real-time data integration flows involves monitoring for events that should trigger the execution of 
services to acquire, transform, or publish data. This is usually implemented within one or multiple proprietary 
technologies and is best implemented with a solution that can manage the operation across technologies. 
2.3.3 Develop Data Migration Approach 
Data needs to be moved when new applications are implemented or when applications are retired or merged. 
This process involves transformation of data to the format of the receiving application. Almost all application 
development projects involve some data migration, even if all that is involved is the population of Reference 
Data. Migration is not quite a one-time process, as it needs to be executed for testing phases as well as final 
implementation. 
Data migration projects are frequently under-estimated or under-designed, because programmers are told to 
simply move the data; they do not engage in the analysis and design activities required for data integration. 
When data is migrated without proper analysis, it often looks different from the data that came in through the 
normal processing. Or the migrated data may not work with the application as anticipated. Profiling data of core 
operational applications will usually highlight data that has been migrated from one or more generations of 
previous operational systems and does not meet the standards of the data that enters the data set through the 
current application code. (See Chapter 6.) 
2.3.4 Develop a Publication Approach 
Systems where critical data is created or maintained need to make that data available to other systems in the 
organization. New or changed data should be pushed by data producing applications to other systems 
(especially data hubs and enterprise data buses) either at the time of data change (event-driven) or on a periodic 
schedule.  
Best practice is to define common message definitions (canonical model) for the various types of data in the 
organization and let data consumers (either applications or individuals) who have appropriate access authority 
subscribe to receive notification of any changes to data of interest. 
2.3.5 Develop Complex Event Processing Flows 
Developing complex event processing solutions requires: 
•
Preparation of the historical data about an individual, organization, product, or market and pre-
population of the predictive models
•
Processing the real-time data stream to fully populate the predictive model and identify meaningful
events (opportunities or threats)
•
Executing the triggered action in response to the prediction
 

