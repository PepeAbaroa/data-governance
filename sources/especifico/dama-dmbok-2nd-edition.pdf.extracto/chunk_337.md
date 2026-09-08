# página 338 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

334 • DMBOK2 
3.4.1 XML 
Extensible Markup Language (XML) provides a language for representing both structured and unstructured data 
and information. XML uses Metadata to describe the content, structure, and business rules of any document or 
database. 
XML requires translating the structure of the data into a document structure for data exchange. XML tags data 
elements to identify the meaning of the data. Simple nesting and references provide the relationships between 
data elements.  
XML namespaces provide a method to avoid a name conflict when two different documents use the same 
element names. Older methods of markup include HTML and SGML, to name a few. 
The need for XML-capable content management has grown for several reasons: 
•
XML provides the capability of integrating structured data into relational databases with unstructured
data. Unstructured data can be stored in a relational DBMS BLOB (binary large object) or in XML
files.
•
XML can integrate structured data with unstructured data in documents, reports, email, images,
graphics, audio, and video files. Data modeling should take into account the generation of unstructured
reports from structured data, and include them in creating error-correction workflows, backup,
recovery, and archiving.
•
XML also can build enterprise or corporate portals, (Business-to-Business [B2B], Business-to-
Customer [B2C]), which provide users with a single access point to a variety of content.
•
XML provides identification and labeling of unstructured data / content so that computer applications
can understand and process them. In this way, structured data appends to unstructured content. An
Extensible Markup Interface (XMI) specification consists of rules for generating the XML document
containing the actual Metadata and thus is a ‘structure’ for XML.
3.4.2 JSON 
JSON (JavaScript Object Notation) is an open, lightweight standard format for data interchange. Its text format 
is language-independent and easy to parse, but uses conventions from the C-family of languages. JSON has two 
structures: a collection of unordered name / value pairs known as objects and an ordered list of values realized 
as an array. It is emerging as the preferred format in web-centric, NoSQL databases.  
An alternative to XML, JSON is used to transmit data between a server and web application. JSON is a similar 
but more compact way of representing, transmitting, and interpreting data than XML. Either XML or JSON 
content can be returned when using REST technology.  
 

