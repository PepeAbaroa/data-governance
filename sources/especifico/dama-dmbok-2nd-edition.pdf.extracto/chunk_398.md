# página 399 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA WAREHOUSING AND BUSINESS INTELLIGENCE • 395 
to ask questions related to capabilities and sources of data to support these capabilities. This time to design pays 
off in reduced rework costs later when the data processing is being tested using the actual data sources. 
In gathering requirements for DW/BI projects, begin with business goals and strategy. Identify and scope the 
business areas, then identify and interview the appropriate business people. Ask what they do and why. Capture 
specific questions they are asking now, and those they want to ask of the data. Document how they distinguish 
between and categorize important aspects of the information. Where possible, define and capture key 
performance metrics and calculations. These can uncover business rules that provide the foundation for 
automation of data quality expectations.  
Catalog requirements and prioritize them into those necessary for production go-live and adoption of the 
warehouse and those that can wait. Look for items that are simple and valuable to jump-start the productivity of 
the initial project release. A DW/BI project requirements write-up should frame the whole context of the 
business areas and / or processes that are in scope. 
2.2 Define and Maintain the DW/BI Architecture 
The DW/BI architecture should describe where data comes from, where it goes, when it goes, why and how it 
goes into a warehouse. The ‘how’ includes the hardware and software detail and the organizing framework to 
bring all the activities together. Technical requirements should include performance, availability, and timing 
needs. (See Chapters 4 and 8.) 
2.2.1 Define DW/BI Technical Architecture 
The best DW/BI architectures will design a mechanism to connect back to transactional level and operational 
level reports in an atomic DW. This mechanism will protect the DW from having to carry every transactional 
detail. An example is providing a viewing mechanism for key operational reports or forms based on a 
transactional key, such as Invoice Number. Customers will always want all the detail available, but some of the 
operational data, such as long description fields, has value only in the context of the original report, and does 
not provide analytic value. 
A conceptual architecture is a starting point. Many activities are necessary to correctly align the non-functional 
requirements to the business needs. Prototyping can quickly prove or disprove key points before making 
expensive commitments to technologies or architectures. In addition, empowering the business community with 
knowledge and adoption programs championed through a sanctioned change management team will assist in 
transition and ongoing operational success.  
A natural extension to this transformation process is the maintenance, or at least validation, with the enterprise 
data model. Since the focus is on which data structures are in use by which organizational areas, check the 
physical deployment against the logical model. Make any updates if omissions or errors arise.  
 

