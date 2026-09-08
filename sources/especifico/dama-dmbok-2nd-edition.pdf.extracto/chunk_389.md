# página 390 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

386 • DMBOK2 
1.3.5 Corporate Information Factory (Inmon) 
Bill Inmon’s Corporate Information Factory (CIF) is one of the two primary patterns for data warehousing. The 
component parts of Inmon’s definition of a data warehouse, “a subject oriented, integrated, time variant, and 
nonvolatile collection of summary and detailed historical data,” describe the concepts that support the CIF and 
point to the differences between warehouses and operational systems.  
•
Subject-oriented: The data warehouse is organized based on major business entities, rather than
focusing on a functional or application.
•
Integrated: Data in the warehouse is unified and cohesive. The same key structures, encoding and
decoding of structures, data definitions, naming conventions are applied consistently throughout the
warehouse. Because data is integrated, Warehouse data is not simply a copy of operational data.
Instead, the warehouse becomes a system of record for the data.
•
Time variant: The data warehouse stores data as it exists in a set point in time. Records in the DW are
like snapshots. Each one reflects the state of the data at a moment of time. This means that querying
data based on a specific time period will always produce the same result, regardless of when the query
is submitted.
•
Non-volatile: In the DW, records are not normally updated as they are in operational systems. Instead,
new data is appended to existing data. A set of records may represent different states of the same
transaction.
•
Aggregate and detail data: The data in the DW includes details of atomic level transactions, as well
as summarized data. Operational systems rarely aggregate data. When warehouses were first
established, cost and space considerations drove the need to summarize data. Summarized data can be
persistent (stored in a table) or non-persistent (rendered in a view) in contemporary DW environments.
The deciding factor in whether to persist data is usually performance.
•
Historical: The focus of operational systems is current data. Warehouses contain historical data as
well. Often they house vast amounts of it.
Inmon, Claudia Imhoff and Ryan Sousa describe data warehousing in the context of the Corporate Information 
Factory (CIF). See Figure 80. CIF components include:  
•
Applications: Applications perform operational processes. Detail data from applications is brought
into the data warehouse and the operational data stores (ODS) where it can be analyzed.
•
Staging Area: A database that stands between the operational source databases and the target
databases. The data staging area is where the extract, transform, and load effort takes place. It is not
used by end users. Most data in the data staging area is transient, although typically there is some
relatively small amount of persistent data.
•
Integration and transformation: In the integration layer, data from disparate sources is transformed
so that it can be integrated into the standard corporate representation / model in the DW and ODS.
 

