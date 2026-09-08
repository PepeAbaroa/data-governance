# página 339 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DOCUMENT AND CONTENT MANAGEMENT • 335 
3.4.3 RDF and Related W3C Specifications 
Resource Description Framework (RDF), a common framework used to describe information about any Web 
resource, is a standard model for data interchange on the Web. The RDF resources are saved in a triplestore, 
which is a database used to store and retrieve semantic queries using SPARQL.  
RDF makes statements about a resource in the form of subject (resource)-predicate (property name)-object 
(property value) expressions or triples. Usually the subject-predicate-object is each described by a URI 
(Uniform Resource Identifier), but the subject and object could be blank nodes and the object could be a literal 
(null values and null strings are not supported). A URI names the relationship between resources as well as two 
ends of the link or triple. The most common form of URI is a URL (uniform resource locator). This allows 
structured and semi-structured data to be shared across applications. 
The Semantic Web needs access to both data and relationships between data sets. The collection of interrelated 
data sets is also known as Linked Data. URIs provide a generic way to identify any entity that exists. HTML 
provides a means to structure and link documents on the Web. RDF provides a generic, graph-based data model 
to link data that describes things.  
RDF uses XML as its encoding syntax. It views Metadata as data (e.g., author, date of creation, etc.). The 
described resources of RDF allow for the association of semantic meanings to resources. RDFS (RDF Schema) 
provides a data modeling vocabulary for RDF data and is an extension of the basic RDF vocabulary. 
SKOS (Simple Knowledge Organization System) is a RDF vocabulary (i.e., an application of the RDF data 
model to capture data depicted as a hierarchy of concepts). Any type of classification, taxonomy, or thesaurus 
can be represented in SKOS. 
OWL (W3C Web Ontology Language) is a vocabulary extension of RDF. It is a semantic markup language for 
publishing and sharing OWL documents (ontologies) on the Web. It is used when information contained in 
documents needs to be processed by applications rather than humans. Both RDF and OWL are Semantic Web 
standards that provide a framework for sharing and reuse of data, as well as enabling data integration and 
interoperability, on the Web. 
RDF can help with the ‘variety’ characteristic of Big Data. If the data is accessible using the RDF triples model, 
data from different sources can be mixed and the SPARQL query language used to find connections and 
patterns without predefining a schema. As W3C describes it, “RDF has features that facilitate data merging 
even if the underlying schemas differ, and it specifically supports the evolution of schemas over time without 
requiring all the data consumers to be changed.”52 It can integrate disparate data from many sources and formats 
and then either reduce or replace the data sets (known as data fusion) through semantic alignment. (See Chapter 
14.) 
52 W3C, “Resource Description Framework (RDF),” http://bit.ly/1k9btZQ. 
 

