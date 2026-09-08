# página 359 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

REFERENCE AND MASTER DATA • 355 
1.3.2.1.3 Taxonomies 
Taxonomic Reference Data structures capture information at different levels of specificity. For example, a US 
ZIP Code may be a meaningful category itself, and it exists within a town, a county, and a state. These 
relationships can be expressed within reference table and multiple levels of analysis could be done using ZIP 
code as a driver.  
Taxonomies enable content classification and multi-faceted navigation to support Business Intelligence. 
Taxonomic Reference Data can be stored in a recursive relationship. Taxonomy management tools also 
maintain hierarchical information. Table 21 and Table 22 show examples of two common hierarchical 
taxonomies. In both cases, the hierarchy includes a code, description, and a reference to a parent code that 
classifies the individual codes. For example, in Table 21, Floral plants (10161600) is a parent code to Roses, 
Poinsettias, and Orchids. In Table 22, Retail Trade (440000) is the parent to Food and Beverage Stores 
(445000), which is the parent to Specialty Food Stores (445200). 
Table 21 UNSPSC (Universal Standard Products and Services Classification)57 
Code Value 
Description 
Parent Code 
10161600 
Floral plants 
10160000 
10161601 
Rose plants 
10161600 
10161602 
Poinsettias plants 
10161600 
10161603 
Orchid plants 
10161600 
10161700 
Cut flowers 
10160000 
10161705 
Cut roses 
10161700 
Table 22 NAICS (North America Industry Classification System)58 
Code Value 
Description 
Parent Code 
440000 
Retail Trade 
440000 
445000 
Food and Beverage Stores 
440000 
445200 
Specialty Food Stores 
445000 
445210 
Meat Markets 
445200 
445220 
Fish and Seafood Markets 
445200 
445290 
Other Specialty Food Stores 
445200 
445291 
Baked Goods Stores 
445290 
445292 
Confectionary and Nut Stores 
445290 
1.3.2.1.4 Ontologies 
Some organizations include ontologies used to manage website content as part of Reference Data. They fit this 
category in that they are used to characterize other data or to relate organizational data to information beyond 
57 http://bit.ly/2sAMU06. 
58 http://bit.ly/1mWACqg. 
 

