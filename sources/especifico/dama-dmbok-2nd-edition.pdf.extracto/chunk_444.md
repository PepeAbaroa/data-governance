# página 445 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

METADATA MANAGEMENT • 441 
Metadata management tools and repositories themselves are also a source of Metadata, especially in a hybrid 
Metadata architectural model or in large enterprise implementations. Metadata management tools allow for the 
exchange of the collected Metadata with other Metadata repositories, enabling the collection of various and 
diverse Metadata from different sources into a centralized repository, or enabling the enriching and 
standardization of the diverse Metadata as it moves between the repositories.  
4. Techniques
4.1 Data Lineage and Impact Analysis 
A key benefit of discovering and documenting Metadata about the physical assets is to provide information on 
how data is transformed as it moves between systems. Many Metadata tools carry information about what is 
happening to the data within their environments and provide capabilities to view the lineage across the span of 
the systems or applications they interface. The current version of the lineage based on programming code is 
referred to as ‘As Implemented Lineage’. In contrast, lineage describe in mapping specification documents is 
referred to as ‘As Designed Lineage’. 
The limitations of a lineage build are based on the coverage of the Metadata management system. Function-
specific Metadata repositories or data visualization tools have information about the data lineage within the 
scope of the environments they interact with but will not provide visibility to what is happening to the data 
outside their environments.  
Metadata management systems import the ‘As Implemented’ lineage from the various tools that can provide 
this lineage detail and then augment the data lineage with the ‘As Designed’ from the places where the actual 
implementation details is not extractable. The process of connecting the pieces of the data lineage referred to as 
stitching. It results in a holistic visualization of the data as it moves from its original locations (official source or 
system of record) until it lands in its final destination. 
Figure 89 shows a sample data element lineage. In reading this, the ‘Total Backorder’ business data element, 
which is physically implemented as column zz_total, depends on 3 other data elements: ‘Units Cost in Cents’ 
physically implemented as ‘yy_unit_cost’, ‘Tax in Ship to State’ implemented in ‘yy_tax’ and ‘Back Order 
Quantity’ implemented in ‘yy_qty’.  
Although a lineage graphic, such as in Figure 89, describes what is happening to a particular data element, not 
all business users will understand it. Higher levels of lineage (e.g., ‘System Lineage’) summarize movement at 
the system or application level. Many visualization tools provide zoom-in / zoom-out capability, to show data 
element lineage in the context of system lineage. For example, Figure 90 shows a sample system lineage, where 
at a glance, general data movement is understood and visualized at a system or an application level.  
 

