# página 187 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

DATA STORAGE AND OPERATIONS • 183 
Due to space and cost, it is usually not possible to exactly replicate production in the pre-production 
environments. The closer on the development path the non-production environment is to the production 
environment, the more closely the non-production environment needs to match the production environment. 
Any deviation from the production system equipment and configuration can itself create issues or errors that are 
unrelated to the change, complicating issue research and resolution. 
Common types of pre-production environments include development, test, support, and special use 
environments.  
1.3.7.2.1 Development 
The development environment is usually a slimmer version of the production environment. It generally has less 
disk space, fewer CPUs, less RAM, etc. Developers use this environment to create and test code for changes in 
separate environments, which then are combined in the QA environment for full integration testing. 
Development can have many copies of production data models, depending on how development projects are 
managed. Larger organizations may give individual developers their own environments to manage with all 
appropriate rights. 
The development environment should be the first place any patches or updates are applied for testing. This 
environment should be isolated from and on different physical hardware than the production environments. Due 
to the isolation, data from production systems may need to be copied to the development environments. 
However, in many industries, production data is protected through regulation. Do not move data from 
production environments without first determining what restrictions there are on doing so. (See Chapter 7.) 
1.3.7.2.2 Test 
The test environment is used to execute quality assurance and user acceptance testing and, in some cases, stress 
or performance tests. In order to prevent test results from being distorted due to environmental differences, the 
test environment ideally also has the same software and hardware as the production environment. This is 
especially important for performance testing. Test may or may not be connected via network to production 
systems in order to read production data. Test environments should never write to production systems.  
Test environments serve many uses: 
•
Quality Assurance Testing (QA): Used to test functionality against requirements.
•
Integration Testing: Used for testing as a whole multiple parts of a system that have been developed
or upgraded independently.
•
User Acceptance Testing (UAT): Used for testing the system functionality from a user perspective.
Use Cases are the most common inputs for testing performed in this environment.
•
Performance Testing: Used to perform high-volume or high-complexity tests at any time, rather than
having to wait for off hours, or adversely affecting production system peak time.
 

