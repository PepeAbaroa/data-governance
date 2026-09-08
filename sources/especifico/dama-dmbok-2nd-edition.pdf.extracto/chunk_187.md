# página 188 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

184 • DMBOK2 
1.3.7.2.3 Sandboxes or Experimental Environments 
A sandbox is an alternate environment that allows read-only connections to production data and can be 
managed by the users. Sandboxes are used to experiment with development options and test hypotheses about 
data or merge production data with user-developed data or supplemental data obtained from external sources. 
Sandboxes are valuable, for example, when performing a Proof-of-Concept.  
A sandbox environment can either be a sub-set of the production system, walled off from production 
processing, or a completely separate environment. Sandbox users often have CRUD rights over their own space 
so that they can quickly validate ideas and options for changes to the system. The DBAs usually have little to do 
with these environments other than setting them up, granting access, and monitoring usage. If the Sandbox areas 
are situated in production database systems, they must be isolated in order to avoid adversely affecting 
production operations. These environments should never write back to the production systems. 
Sandbox environments could be handled by virtual machines (VMs), unless licensing costs for separate 
instances becomes prohibitive. 
1.3.8 Database Organization 
Data storage systems provide a way to encapsulate the instructions necessary to put data on disks and manage 
processing, so developers can simply use instructions to manipulate data. Databases are organized in three 
general ways: Hierarchical, Relational, and Non-Relational. These classes are not mutually exclusive (see 
Figure 59). Some database systems can read and write data organized in relational and non-relational structures. 
Hierarchical databases can be mapped to relational tables. Flat files with line delimiters can be read as tables 
with rows, and one or more columns can be defined to describe the row contents. 
Figure 59 Database Organization Spectrum 
1.3.8.1 Hierarchical 
Hierarchical database organization is the oldest database model, used in early mainframe DBMS, and is the 
most rigid of structures. In hierarchical databases, data is organized into a tree-like structure with mandatory 
More Controlled Structure
Less Controlled Structure
RELATIONAL
(Schema on 
Write)
HIERARCHICAL 
(Tree Schema)
NON-
RELATIONAL
(Schema on 
Read)
 

