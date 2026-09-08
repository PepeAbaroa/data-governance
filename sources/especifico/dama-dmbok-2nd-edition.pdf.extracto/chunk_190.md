# página 191 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 187 
layouts are well suited for Online Analytical Processing (OLAP)-like workloads (e.g., data 
warehouses) which typically involve a smaller number of highly complex queries over all data 
(possibly terabytes). 
1.3.8.3.2 Spatial 
A spatial database is optimized to store and query data that represents objects defined in a geometric space. 
Spatial databases support several primitive types (simple geometric shapes such as box, rectangle, cube, 
cylinder, etc.) and geometries composed of collections of points, lines, and shapes.  
Spatial database systems use indexes to quickly look up values; the way that most databases index data is not 
optimal for spatial queries. Instead, spatial databases use a spatial index to speed up database operations.  
Spatial databases can perform a wide variety of spatial operations. As per the Open Geospatial Consortium 
standard, a spatial database may perform one or more of the following operations:  
•
Spatial Measurements: Computes line length, polygon area, the distance between geometries, etc.
•
Spatial Functions: Modifies existing features to create new ones; for example, by providing a buffer
around them, intersecting features, etc.
•
Spatial Predicates: Allows true/false queries about spatial relationships between geometries.
Examples include “Do two polygons overlap?” or “Is there a residence located within a mile of the
area of the proposed landfill?”
•
Geometry Constructors: Creates new geometries, usually by specifying the vertices (points or nodes)
which define the shape.
•
Observer Functions: Queries that return specific information about a feature such as the location of
the center of a circle.
1.3.8.3.3 Object / Multi-media 
A multimedia database includes a Hierarchical Storage Management system for the efficient management of a 
hierarchy of magnetic and optical storage media. It also includes a collection of objects classes, which 
represents the foundation of the system.  
1.3.8.3.4 Flat File Database 
A flat file database describes any of various means to encode a data set as a single file. A flat file can be a plain 
text file or a binary file. Strictly, a flat file database consists of nothing but data, and contains records that may 
vary in length and delimiters. More broadly, the term refers to any database that exists in a single file in the 
 

