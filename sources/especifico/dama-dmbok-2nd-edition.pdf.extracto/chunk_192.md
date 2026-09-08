# página 193 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 189 
•
Computer Assisted Design and Manufacturing (CAD / CAM) applications require an Object
database, as will most embedded real-time applications.
•
Geographical Information Systems (GIS) make use of specialized geospatial databases, which have
at least annual updates to their Reference Data. Some specialized GIS are used for utilities (electric
grid, gas lines, etc.), for telecom in network management, or for ocean navigation.
•
Shopping-cart applications found on most online retail websites, make use of XML databases to
initially store the customer order data, and may be used real-time by social media databases for ad
placement on other websites.
Some of this data is then copied into one or more traditional OLTP (Online Transaction Processing) databases 
or data warehouses. In addition, many off-the-shelf vendor applications may use their own proprietary 
databases. At the very least, their schemas will be proprietary and mostly concealed, even if they sit on top of 
traditional relational DBMSs. 
1.3.10 Common Database Processes 
All databases, no matter the type, share the following processes in some way. 
1.3.10.1 Archiving 
Archiving is the process of moving data off immediately accessible storage media and onto media with lower 
retrieval performance. Archives can be restored to the originating system for short-term use. Data that is not 
actively needed to support application processes should be moved to an archive on less-expensive disk, tape, or 
a CD / DVD jukebox. Restoring from an archive should be a matter of simply copying the data from the archive 
back into the system. 
Archival processes must be aligned with the partitioning strategy to ensure optimal availability and retention. A 
robust approach involves: 
•
Creating a secondary storage area, preferably on a secondary database server
•
Partitioning existing database tables into archival blocks
•
Replicating the data that is needed less often to the separate database
•
Creating tape or disk backups
•
Creating database jobs that periodically purge unneeded data
It is wise to schedule regular tests of archive restoration to ensure avoid surprises in an emergency. 
When changes are made to the technology or structure of a production system, the archive also needs to be 
evaluated to ensure that data moved from the archive into current storage will be readable. There are several 
ways of handling out-of-synch archives: 
 

