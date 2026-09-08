# página 491 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA QUALITY • 487 
•
Automated correction: Automated correction techniques include rule-based standardization,
normalization, and correction. The modified values are obtained or generated and committed without
manual intervention. An example is automated address correction, which submits delivery addresses to
an address standardizer that conforms and corrects delivery addresses using rules, parsing,
standardization, and reference tables. Automated correction requires an environment with well-defined
standards, commonly accepted rules, and known error patterns. The amount of automated correction
can be reduced over time if this environment is well-managed and corrected data is shared with
upstream systems.
•
Manually-directed correction: Use automated tools to remediate and correct data but require manual
review before committing the corrections to persistent storage. Apply name and address remediation,
identity resolution, and pattern-based corrections automatically, and use some scoring mechanism to
propose a level of confidence in the correction. Corrections with scores above a particular level of
confidence may be committed without review, but corrections with scores below the level of
confidence are presented to the data steward for review and approval. Commit all approved
corrections, and review those not approved to understand whether to adjust the applied underlying
rules. Environments in which sensitive data sets require human oversight (e.g., MDM) are good
examples of where manual-directed correction may be suited.
•
Manual correction: Sometimes manual correction is the only option in the absence of tools or
automation or if it is determined that the change is better handled through human oversight. Manual
corrections are best done through an interface with controls and edits, which provide an audit trail for
changes. The alternative of making corrections and committing the updated records directly in
production environments is extremely risky. Avoid using this method.
4.3 Quality Check and Audit Code Modules 
Create shareable, linkable, and re-usable code modules that execute repeated data quality checks and audit 
processes that developers can get from a library. If the module needs to change, then all the code linked to that 
module will get updated. Such modules simplify the maintenance process. Well-engineered code blocks can 
prevent many data quality problems. As importantly, they ensure processes are executed consistently. Where 
laws or policy mandate reporting of specific quality results, the lineage of results often needs to be described. 
Quality check modules can provide this. For data that has any questionable quality dimension and that is highly 
rated, qualify the information in the shared environments with quality notes, and confidence ratings.  
4.4 Effective Data Quality Metrics 
A critical component of managing data quality is developing metrics that inform data consumers about quality 
characteristics that are important to their uses of data. Many things can be measured, but not all of them are 
worth the time and effort. In developing metrics, DQ analysts should account for these characteristics:  
 

