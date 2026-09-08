# página 266 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

262 • DMBOK2 
4.6 Efficient Search of Encrypted Data 
Searching encrypted data obviously includes the need to decrypt the data. One way to reduce the amount of data 
that needs decryption is to encrypt the search criteria (such as a string) using the same encryption method used 
for the data, and then seek matches. The amount of data matching the encrypted search criteria will be much 
less, and therefore less costly (and risky) to decrypt. Then search using clear text on the result set to get exact 
matches. 
4.7 Document Sanitization 
Document sanitization is the process of cleaning Metadata, such as tracked change history, from documents 
before sharing. Sanitization mitigates the risk of sharing confidential information that might be embedded in 
comments. In contracts especially, access to this information may negatively affect negotiations. 
5. Implementation Guidelines
Implementation of data security practices depends on corporate culture, the nature of the risks, the sensitivity of 
what data the company manages, and the types of systems in place. Implementation system components should 
be guided by a strategic security plan and supporting architecture.  
5.1 Readiness Assessment / Risk Assessment 
Keeping data secure is deeply connected to corporate culture. Organizations often end up reacting to crises, 
rather than proactively managing accountability and ensuring auditability. While perfect data security is next to 
impossible, the best way to avoid data security breaches is to build awareness and understanding of security 
requirements, policies, and procedures. Organizations can increase compliance through: 
•
Training: Promotion of standards through training on security initiatives at all levels of the
organization. Follow training with evaluation mechanisms such as online tests focused on improving
employee awareness. Such training and testing should be mandatory and a prerequisite for employee
performance evaluation.
•
Consistent policies: Definition of data security policies and regulatory compliance policies for
workgroups and departments that complement and align with enterprise policies. Adopting an ‘act
local’ mindset helps engage people more actively.
•
Measure the benefits of security: Link data security benefits to organizational initiatives.
Organizations should include objective metrics for data security activities in their balanced scorecard
measurements and project evaluations.
 

