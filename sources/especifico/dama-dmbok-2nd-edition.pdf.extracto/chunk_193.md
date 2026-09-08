# página 194 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

190 • DMBOK2 
•
Determine if or how much of the archive is required to be preserved. What is not required can be
considered purged.
•
For major changes in technology, restore the archives to the originating system before the technology
change, upgrade or migrate to the new technology, and re-archive the data using the new technology.
•
For high-value archives where the source database structures change, restore the archive, make any
changes to the data structures, and re-archive the data with the new structure.
•
For infrequent-access archives where the source technology or structure changes, keep a small version
of the old system running with limited access, and extract from the archives using the old system as
needed.
Archives that are not recoverable with current technology are useless, and keeping old machinery around to 
read archives that cannot be otherwise read, is not efficient or cost-effective. 
1.3.10.2 Capacity and Growth Projections 
Think of a database as a box, the data as fruit, and overhead (indexes, etc.) as packing material. The box has 
dividers, and fruit and packing material go in the cells:  
•
First, decide the size of the box that will hold all the fruit and any packing material needed – that is the
Capacity.
•
How much fruit goes into the box, and how quickly?
•
How much fruit comes out of the box, and how quickly?
Decide if the box will stay the same size over time, or must be expanded over time to hold more fruit. This 
projection of how much and how quickly the box must expand to hold incoming fruit and packing material is 
the growth projection. If the box cannot expand, the fruit must be taken out as fast as it is put in, and the growth 
projection is zero. 
How long should the fruit stay in the cells? If the fruit in one cell gets dehydrated over time, or for any reason 
becomes not as useful, should that fruit be put in a separate box for longer term storage (i.e., archived)? Will 
there ever be a need to bring that dehydrated fruit back into the main box? Moving the fruit to another box with 
the ability to move it back into the first box is an important part of archiving. This allows the box to not have to 
be expanded quite as often or as much. 
If a fruit becomes too stagnant to use, throw that fruit away (i.e., purge the data). 
1.3.10.3 Change Data Capture (CDC) 
Change data capture refers to the process of detecting that data has changed and ensuring that information 
relevant to the change is stored appropriately. Often referred to as log-based replication, CDC is a non-invasive 
 

