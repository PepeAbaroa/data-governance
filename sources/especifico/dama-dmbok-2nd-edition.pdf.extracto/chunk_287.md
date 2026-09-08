# página 288 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

284 • DMBOK2 
The goal of service-oriented architecture is to have well-defined interaction between self-contained software 
modules. Each module performs functions (a.k.a. provides services) to other software modules or to human 
consumers. The key concept is that SOA architecture provides independent services: the service has no fore 
knowledge of the calling application and the implementation of the service is a black box to the calling 
application. A service-oriented architecture may be implemented with various technologies including web 
services, messaging, RESTful APIs, etc. Services are usually implemented as APIs (application programming 
interfaces) that are available to be called by application systems (or human consumers). A well-defined API 
registry describes what options are available, parameters that need to be provided, and resulting information that 
is provided. 
Data services, which may include the addition, deletion, update, and retrieval of data, are specified in a catalog 
of available services. To achieve the enterprise goals of scalability (supporting integrations between all 
applications in the enterprise without using unreasonable amounts of resources to do so) and reuse (having 
services that are leveraged by all requestors of data of a type), a strong governance model must be established 
around the design and registration of services and APIs. Prior to developing new data services, it is necessary to 
ensure that no service already exists that could provide the requested data. In addition, new services need to be 
designed to meet broad requirements so that they will not be limited to the immediate need but can be reused. 
1.3.7.6 Complex Event Processing (CEP) 
Event processing is a method of tracking and analyzing (processing) streams of information (data) about things 
that happen (events), and deriving a conclusion from them. Complex event processing (CEP) combines data 
from multiple sources to identify meaningful events (such as opportunities or threats) to predict behavior or 
activity and automatically trigger real-time response, such as suggesting a product for a consumer to purchase. 
Rules are set to guide the event processing and routing.  
Organizations can use complex event processing to predict behavior or activity and automatically trigger real-
time response. Events such as sales leads, web clicks, orders, or customer service calls may happen across the 
various layers of an organization. Alternatively, they may include news items, text messages, social media 
posts, stock market feeds, traffic reports, weather reports, or other kinds of data. An event may also be defined 
as a change of state, when a measurement exceeds a predefined threshold of time, temperature, or other value.  
CEP presents some data challenges. In many cases, the rate at which events occur makes it impractical to 
retrieve the additional data necessary to interpret the event as it occurs. Efficient processing typically mandates 
pre-positioning some data in the CEP engine’s memory.  
Supporting complex event processing requires an environment that can integrate vast amounts of data of various 
types. Because of the volume and variety of data usually involved in creating predictions, complex event 
processing is often tied to Big Data. It often requires use of technologies that support ultra-low latency 
requirements such as processing real-time streaming data and in-memory databases. (See Chapter 14.) 
 

