# página 192 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

188 • DMBOK2 
form of rows and columns, with no relationships or links between records and fields except the structure. Plain 
text files usually contain one record per line. A list of names, addresses, and phone numbers, written by hand on 
a sheet of paper, is an example of a flat file database. Flat files are used not only as data storage tools in DBMS 
systems, but also as data transfer tools. Hadoop databases use flat file storage. 
1.3.8.3.5 Key-Value Pair 
Key-Value pair databases contain sets of two items: a key identifier and a value. There are a few specific uses 
of these types of databases. 
•
Document Databases: Document-oriented databases contain collections of files including both
structure and data. Each document is assigned a key. More advanced document-oriented databases also
can store attributes for the document’s contents, such as dates or tags. This type of database can store
both complete and incomplete documents. Document databases may use XML or JSON (Java Script
Object Notation) structures.
•
Graph Databases: Graph databases store key-value pairs where the focus is on the relationship
between the nodes, rather than on the nodes themselves.
1.3.8.3.6 Triplestore 
A data entity composed of subject-predicate-object is known as a triplestore. In Resource Description 
Framework (RDF) terminology, a triplestore is composed of a subject that denotes a resource, the predicate that 
expresses a relationship between the subject and the object, and the object itself. A triplestore is a purpose-built 
database for the storage and retrieval of triples in the form of subject-predicate-object expressions.  
Triplestores can be broadly classified into three categories: Native triplestores, RDBMS-backed triplestores and 
NoSQL triplestores. 
•
Native triplestores are those that are implemented from scratch and exploit the RDF data model to
efficiently store and access the RDF data.
•
RDBMS-backed triplestores are built by adding an RDF specific layer to an existing RDBMS.
•
NoSQL Triplestores are currently being investigated as possible storage managers for RDF.
Triplestore databases are best for taxonomy and thesaurus management, linked data integration, and knowledge 
portals. 
1.3.9 Specialized Databases 
Some specialized situations require specialized types of databases that are managed differently from traditional 
relational databases. Examples include: 
 

