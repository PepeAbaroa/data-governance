# página 232 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

228 • DMBOK2 
environments. Persistent masking changes the data, but the data must still be viable for use to test processes, 
application, report, etc. 
•
In-flight persistent masking occurs when the data is masked or obfuscated while it is moving
between the source (typically production) and destination (typically non-production) environment. In-
flight masking is very secure when properly executed because it does not leave an intermediate file or
database with unmasked data. Another benefit is that it is re-runnable if issues are encountered part
way through the masking.
•
In-place persistent masking is used when the source and destination are the same. The unmasked data
is read from the source, masked, and then used to overwrite the unmasked data. In-place masking
assumes the sensitive data is in a location where it should not exist and the risk needs to be mitigated,
or that there is an extra copy of the data in a secure location to mask before moving it to the non-secure
location. There are risks to this process. If the masking process fails mid-masking, it can be difficult to
restore the data to a useable format. This technique has a few niche uses, but in general, in-flight
masking will more securely meet project needs.
1.3.9.2 Dynamic Data Masking 
Dynamic data masking changes the appearance of the data to the end user or system without changing the 
underlying data. This can be extremely useful when users need access to some sensitive production data, but not 
all of it. For example, in a database the social security number is stored as 123456789, but to the call center 
associate that needs to verify who they are speaking to, the data shows up as ***-**-6789. 
1.3.9.3 Masking Methods 
There are several methods for masking or obfuscating data. 
•
Substitution: Replace characters or whole values with those in a lookup or as a standard pattern. For
example, first names can be replaced with random values from a list.
•
Shuffling: Swap data elements of the same type within a record, or swap data elements of one attribute
between rows. For example, mixing vendor names among supplier invoices such that the original
supplier is replaced with a different valid supplier on an invoice.
•
Temporal variance: Move dates +/– a number of days – small enough to preserve trends, but
significant enough to render them non-identifiable.
•
Value variance: Apply a random factor +/– a percent, again small enough to preserve trends, but
significant enough to be non-identifiable.
•
Nulling or deleting: Remove data that should not be present in a test system.
 

