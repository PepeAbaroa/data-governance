# página 64 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

60 • DMBOK2 
•
Unreliable Metadata: Data consumers depend on reliable Metadata, including consistent definitions of
individual data elements, documentation of data’s origin, and documentation of lineage (e.g., rules by
which data is integrated). Without reliable Metadata, data may be misunderstood and potentially misused.
In cases where data may move between organizations and especially where it may move across borders,
Metadata should include tags that indicate its provenance, who owns it, and if it requires specific
protection.
•
No documentation of data remediation history: Organizations should also have auditable information
related to the ways data has been changed. Even if the intention of data remediation is to improve the
quality of data, doing so may be illegal. Data remediation should always follow a formal, auditable change
control process.
3.4.6 Obfuscation / Redaction of Data 
Obfuscating or redacting data is the practice of making information anonymous, or removing sensitive information. 
But obfuscation alone may not be sufficient to protect data if a downstream activity (analysis or combination with 
other datasets) can expose the data. This risk is present in the following instances: 
•
Data aggregation: When aggregating data across some set of dimensions, and removing identifying data,
a dataset can still serve an analytic purpose without concern for disclosing personal identifying
information (PII). Aggregations into geographic areas are a common practice (see Chapters 7 and 14).
•
Data marking: Data marking is used to classify data sensitivity (secret, confidential, personal, etc.) and to
control release to appropriate communities such as the public or vendors, or even vendors from certain
countries or other community considerations.
•
Data masking: Data masking is a practice where only appropriate submitted data will unlock processes.
Operators cannot see what the appropriate data might be; they simply type in responses given to them, and
if those responses are correct, further activities are permitted. Business processes using data masking
include outsourced call centers, or sub-contractors who should only have partial access to information.
The use of extremely large data sets in Data Science analyses raises practical rather than merely theoretical 
concerns about the effectiveness of anonymization. Within large data sets, it is possible to combine data in ways 
enable individuals to be specifically identified, even if input data sets have been anonymized. The first concern 
when data lands in a data lake is to analyze it for sensitive data and apply accepted protection methods. These alone 
may not offer enough safeguard, however; this is why it is vital that organizations have strong governance and a 
commitment to ethical data handling. (See Chapter 14.)  
3.5 Establishing an Ethical Data Culture 
Establishing a culture of ethical data handling requires understanding existing practices, defining expected 
behaviors, codifying these in policies and a code of ethics, and providing training and oversight to enforce expected 

