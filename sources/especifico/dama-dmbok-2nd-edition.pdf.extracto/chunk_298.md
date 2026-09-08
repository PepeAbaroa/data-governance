# página 299 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA INTEGRATION AND INTEROPERABILITY • 295 
The enterprise service bus implements incoming and outgoing message queues on each of the systems 
participating in message interchange with an adapter or agent installed in each environment. The central 
processor for the ESB is usually implemented on a server separate from the other participating systems. The 
processor keeps track of which systems have subscribed interest in what kinds of messages. The central 
processor continuously polls each participating system for outgoing messages and deposits incoming messages 
into the message queue for subscribed types of messages and messages that have been directly addressed to that 
system.  
This model is called ‘near real-time’ because the data can take up to a couple of minutes to get from sending 
system to receiving system. This is a loosely coupled model and the system sending data will not wait for 
confirmation of receipt and update from the receiving system before continuing processing. 
3.4 Business Rules Engine 
Many data integration solutions are dependent on business rules. An important form of Metadata, these rules 
can be used in basic integration and in solutions that incorporate complex event processing to enable an 
organization to respond to events in near real-time. A business rules engine that allows non-technical users to 
manage business rules implemented by software is a very valuable tool that will enable evolution of the solution 
at a lower cost, because a business rules engine can support changes to predictive models without technical code 
changes. For example, models that predict what a customer might want to purchase may be defined as business 
rules rather than code changes. 
3.5 Data and Process Modeling Tools 
Data modeling tools should be used to design not only the target but also the intermediate data structures needed 
in data integration solutions. The structure of the messages or streams of data that pass between systems and 
organizations, and are not usually persisted, should nevertheless be modeled. The flow of data between systems 
and organizations should also be designed, as should complex event processes. 
3.6 Data Profiling Tool 
Data profiling involves statistical analysis of data set contents to understand format, completeness, consistency, 
validity, and structure of the data. All data integration and interoperability development should include detailed 
assessment of potential data sources and targets to determine whether the actual data meets the needs of the 
proposed solution. Since most integration projects involve a significant amount of data, the most efficient 
means of conducting this analysis is to use a data profiling tool. (See Section 2.1.4 and Chapter 13.) 
 

