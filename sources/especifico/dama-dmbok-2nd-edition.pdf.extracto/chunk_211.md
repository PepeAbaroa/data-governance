# página 212 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

208 • DMBOK2 
Test data is data that has been specifically identified to test a system. Testing can include verifying that a given 
set of input produces expected output or challenging the ability of programming to respond to unusual, extreme, 
exceptional, or unexpected input. Test data can be completely fabricated or generated using meaningless values 
or it can be sample data. Sample data can be a subset of actual production data (by either content or structure), 
or generated from production data. Production data can be filtered or aggregated to create multiple sample data 
sets, depending on the need. In cases where production data contains protected or restricted data, sample data 
must be masked.  
Test data may be produced in a focused or systematic way (as is typically the case in functionality testing) using 
statistics or filters, or by using other, less-focused approaches (as is typically the case in high-volume 
randomized automated tests). Test data may be produced by the tester, by a program or function that aids the 
tester, or by a copy of production data that has been selected and screened for the purpose. Test data may be 
recorded for short-term re-use, created and managed to support regression tests, or used once and then removed 
– although in most organizations, cleanup after projects does not include this step. DBAs should monitor project
test data and ensure that obsolete test data is purged regularly to preserve capacity. 
It is not always possible to produce enough data for some tests, especially performance tests. The amount of test 
data to be generated is determined or limited by considerations such as time, cost, and quality. It is also 
impacted by regulation that limits the use of production data in a test environment. (See Chapter 7.) 
2.2.6 Manage Data Migration 
Data migration is the process of transferring data between storage types, formats, or computer systems, with as 
little change as possible. Changing data during migration is discussed in Chapter 8. 
Data migration is a key consideration for any system implementation, upgrade, or consolidation. It is usually 
performed programmatically, being automated based on rules. However, people need to ensure that the rules 
and programs are executed correctly. Data migration occurs for a variety of reasons, including server or storage 
equipment replacements or upgrades, website consolidation, server maintenance, or data center relocation. Most 
implementations allow this to be done in a non-disruptive manner, such as concurrently while the host continues 
to perform I/O to the logical disk (or LUN). 
The mapping granularity dictates how quickly the Metadata can be updated, how much extra capacity is 
required during the migration, and how quickly the previous location is marked as free. Smaller granularity 
means faster update, less space required, and quicker freeing up of old storage. 
Many day-to-day tasks a storage administrator has to perform can be simply and concurrently completed using 
data migration techniques: 
•
Moving data off an over-used storage device to a separate environment
•
Moving data onto a faster storage device as needs require
•
Implementing an Information Lifecycle Management policy
•
Migrating data off older storage devices (either being scrapped or off-lease) to offline or cloud storage
 

