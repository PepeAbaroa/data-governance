# página 118 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

114 • DMBOK2 
to be shareable or reusable need to be incorporated into the enterprise logical data model and 
designated repositories.  
•
Understand business requirements: Capture data-related requirements such as entity, source(s),
availability, quality, and pain points, and estimate the business value of meeting these requirements.
•
Design: Form detailed target specifications, including business rules in a data lifecycle perspective.
Validate the outcome and, when needed, address needs for extended and improved standardized
models. The enterprise logical data model and enterprise architecture repository are good places for
project data architects to look and reuse constructs that are shareable across the enterprise. Review and
use data technology standards.
•
Implement:
o
When buying, reverse engineer purchased applications (Commercial Off the Shelf – COTS)
and map against data structure. Identify and document gaps and differences in structures,
definitions, and rules. Ideally, vendors will supply data models for their products; however,
many do not, as they consider these proprietary. If possible, negotiate for a model with in-
depth definitions.
o
When reusing data, map application data models against common data structures and
existing and new processes to understand CRUD operations. Enforce the use of system of
record or other authoritative data. Identify and document gaps.
o
When building, implement data storage according to the data structure. Integrate according
to standardized or designed specifications. (See Chapter 8.)
The role of Enterprise Data Architects in projects depends on the development methodology. The process of 
building architectural activities into projects also differs between methodologies. 
•
Waterfall methods: Understand the requirements and construct systems in sequential phases as part of
an overall enterprise design. This method includes tollgates designed to control change. It is usually no
problem to include Data Architecture activities in such models. Be sure to include an enterprise
perspective.
•
Incremental methods: Learn and construct in gradual steps (i.e., mini-waterfalls). This method creates
prototypes based on vague overall requirements. The initiation phase is crucial; it is best to create a
comprehensive data design in early iterations.
•
Agile, iterative, methods: Learn, construct, and test in discrete delivery packages (called ‘sprints’)
that are small enough that if work needs to be discarded, not much is lost. Agile methods (Scrum,
Rapid Development, and Unified Process) promote object-oriented modeling that emphasizes user
interface design, software design, and systems behavior. Complete such methods with specifications
for data models, data capture, data storage, and data distribution. Experience from DevOps, an
emerging and popular agile approach, testifies about improved data design and effective design choices
when programmers and data architects have a strong working relationship and both comply with
standards and guidelines.

