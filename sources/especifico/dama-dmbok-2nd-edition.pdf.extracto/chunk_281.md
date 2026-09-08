# página 282 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

278 • DMBOK2 
of the applications that need the update are not available then the transaction cannot be completed in the 
primary application. This situation keeps data synchronized but has the potential to make strategic applications 
dependent on less critical applications.  
Solutions using this type of architecture exist on a continuum based on how much difference between data sets 
might be possible and how much such a solution is worth. Data sets may be kept in synch through database 
capabilities such as two-phase commits, which ensure that all updates in a business transaction are all 
successful, or none is made. For example, financial institutions use two-phase commit solutions to ensure that 
financial transaction tables are absolutely synchronized with financial balance tables. Most programming does 
not use two-phase commit. There is a very small possibility that if an application is interrupted unexpectedly 
then one data set may be updated but not another.  
Real-time, synchronous solutions require less state management than asynchronous solutions because the order 
in which transactions are processed is clearly managed by the updating applications. However, they also may 
lead to blocking and delay other transactions. 
1.3.2.6 Low Latency or Streaming 
Tremendous advances have been made in developing extremely fast data integration solutions. These solutions 
require a large investment in hardware and software. The extra costs of low latency solutions are justified if an 
organization requires extremely fast data movement across large distances. ‘Streaming data’ flows from 
computer systems on a real-time continuous basis immediately as events occur. Data streams capture events like 
the purchase of goods or financial securities, social media comments, and readouts from sensors monitoring 
location, temperature, usage, or other values.  
Low latency data integration solutions are designed to minimize the response time to events. They may include 
the use of hardware solutions like solid-state disk or software solutions like in-memory databases so that the 
process does not have to slow down to read or write to traditional disk. The read and write processes to 
traditional disk drives is thousands of times slower than processing data in-memory or on solid-state disk drives. 
Asynchronous solutions are usually used in low latency solutions so that transactions do not need to wait for 
confirmation from subsequent processes before processing the next piece of data.  
Massive multi-processing, or simultaneous processing, is also a common configuration in low latency solutions 
so that the processing of incoming data can be spread out over many processors simultaneously, and not 
bottlenecked by a single or small number of processors. 
1.3.3 Replication 
To provide better response time for users located around the world, some applications maintain exact copies of 
data sets in multiple physical locations. Replication solutions minimize the performance impact of analytics and 
queries on the primary transactional operating environment.  
 

