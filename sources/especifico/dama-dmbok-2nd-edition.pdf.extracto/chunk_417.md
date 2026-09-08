# página 418 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

414 • DMBOK2 
Mapping operational source(s) to targets is another natural extension, which enforces and validates the lineage 
and Metadata already collected, and can provide penetration analysis for which source systems are in analytical 
use by which departments. This can help focus tuning efforts on those high impact analytic queries by 
mitigating any changes to heavily used sourced objects. 
6.5.3 Response and Performance Metrics 
Most query tools measure response time. Retrieve response or performance metrics from tools. This data will 
inform metrics about the number and type of users.  
Harvest load times for each data product in raw format from the population processes. These should also be 
expressed as a percentage of expected support: so a mart that is expected to be refreshed daily and loaded in a 
four-hour window is 100% supported when it loads in four hours. Apply this process to any extracts generated 
for downstream processing too. 
Most tools will retain, in a log or repository, query records, data refresh, and data extract times for the objects 
provided to the users. Divide this data into scheduled and executed objects, and express as raw counts both 
attempted and succeeded. Highly popular objects or queries performing poorly are likely in-need of attention 
before satisfaction metrics suffer. This can guide defect analysis, maintenance planning, as well as capacity 
planning if a group of objects is failing regularly. Remediation may vary depending on the tool, but sometimes 
creating or dropping one index can result in great improvements. (See Chapter 6.) 
A natural follow on for this is the validation and adjustment of service levels. Adjust items that have 
consistently failed in the next release, or in the absence of necessary funding, the support level must be reduced. 
7. Works Cited / Recommended
Adamson, Christopher. Mastering Data Warehouse Aggregates: Solutions for Star Schema Performance. John Wiley and 
Sons, 2006. Print. 
Adelman, Sid and Larissa T. Moss. Data Warehouse Project Management. Addison-Wesley Professional, 2000. Print. 
Adelman, Sid, Larissa Moss and Majid Abai. Data Strategy. Addison-Wesley Professional, 2005. Print. 
Adelman, Sid, et al. Impossible Data Warehouse Situations: Solutions from the Experts. Addison-Wesley, 2002. Print. 
Aggarwal, Charu. Data Mining: The Textbook. Springer, 2015. Print. 
Biere, Mike. Business Intelligence for the Enterprise. IBM Press, 2003. Print. 
Biere, Mike. The New Era of Enterprise Business Intelligence: Using Analytics to Achieve a Global Competitive Advantage. 
IBM Press, 2010. Print. IBM Press. 
Brown, Meta S. Data Mining for Dummies. For Dummies, 2014. Print. For Dummies. 
Chorianopoulos, Antonios. Effective CRM using Predictive Analytics. Wiley, 2016. Print. 
 

