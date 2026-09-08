# página 131 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA MODELING AND DESIGN • 127 
•
Resource information: Basic profiles of resources needed conduct operational processes such as
Product, Customer, Supplier, Facility, Organization, and Account. Among IT professionals, resource
entities are sometimes referred to as Reference Data.
•
Business event information: Data created while operational processes are in progress. Examples
include Customer Orders, Supplier Invoices, Cash Withdrawal, and Business Meetings. Among IT
professionals, event entities are sometimes referred to as transactional business data.
•
Detail transaction information: Detailed transaction information is often produced through point-of-
sale systems (either in stores or online). It is also produced through social media systems, other
Internet interactions (clickstream, etc.), and by sensors in machines, which can be parts of vessels and
vehicles, industrial components, or personal devices (GPS, RFID, Wi-Fi, etc.). This type of detailed
information can be aggregated, used to derive other data, and analyzed for trends, similar to how the
business information events are used. This type of data (large volume and/or rapidly changing) is
usually referred to as Big Data.
These types refer to ‘data at rest’. Data in motion can also be modeled, for example, in schemes for systems, 
including protocols, and schemes for messaging and event-based systems. 
1.3.3 Data Model Components 
As will be discussed later in the chapter, different types of data models represent data through different 
conventions (See Section 1.3.4). However, most data models contain the same basic building blocks: entities, 
relationships, attributes, and domains.  
1.3.3.1 Entity 
Outside of data modeling, the definition of entity is a thing that exists separate from other things. Within data 
modeling, an entity is a thing about which an organization collects information. Entities are sometimes referred 
to as the nouns of an organization. An entity can be thought of as the answer to a fundamental question – who, 
what, when, where, why, or how – or to a combination of these questions (see Chapter 4). Table 7 defines and 
gives examples of commonly used entity categories (Hoberman, 2009). 
Table 7 Commonly Used Entity Categories 
Category 
Definition 
Examples 
Who 
Person or organization of interest. That is, Who is 
important to the business? Often a ‘who’ is associated 
with a party generalization, or role such as Customer or 
Vendor. Persons or organizations can have multiple 
roles or be included in multiple parties. 
Employee, Patient, Player, Suspect, 
Customer, Vendor, Student, 
Passenger, Competitor, Author  
 

