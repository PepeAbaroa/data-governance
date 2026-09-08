# página 506 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

502 • DMBOK2 
•
Acquire and ingest data sources: Obtain data sets and onboard them.
•
Develop Data Science hypotheses and methods: Explore data sources via profiling, visualization,
mining, etc.; refine requirements. Define model algorithm inputs, types, or model hypotheses and
methods of analysis (i.e., groupings of data found by clustering, etc.).
•
Integrate and align data for analysis: Model feasibility depends in part on the quality of the source
data. Leverage trusted and credible sources. Apply appropriate data integration and cleansing
techniques to increase quality and usefulness of provisioned data sets.
•
Explore data using models: Apply statistical analysis and machine learning algorithms against the
integrated data. Validate, train, and over time, evolve the model. Training entails repeated runs of the
model against actual data to verify assumptions and make adjustments, such as identifying outliers.
Through this process, requirements will be refined. Initial feasibility metrics guide evolution of the
model. New hypotheses may be introduced that require additional data sets and results of this
exploration will shape the future modeling and outputs (even changing the requirements).
•
Deploy and monitor: Those models that produce useful information can be deployed to production for
ongoing monitoring of value and effectiveness. Often Data Science projects turn into data warehousing
projects where more vigorous development processes are put in place (ETL, DQ, Master Data, etc.).
1.3.3 Big Data 
Early efforts to define the meaning of Big Data characterized it in terms of the Three V’s: Volume, Velocity, 
Variety (Laney, 2001). As more organizations start to leverage the potential of Big Data, the list of V’s has 
expanded: 
•
Volume: Refers to the amount of data. Big Data often has thousands of entities or elements in billions
of records.
•
Velocity: Refers to the speed at which data is captured, generated, or shared. Big Data is often
generated and can also be distributed and even analyzed in real-time.
•
Variety / Variability: Refers to the forms in which data is captured or delivered. Big Data requires
storage of multiple formats; data structure is often inconsistent within or across data sets.
•
Viscosity: Refers to how difficult the data is to use or integrate.
•
Volatility: Refers to how often data changes occur and therefore how long the data is useful.
•
Veracity: Refers to how trustworthy the data is.
Big Data volumes are exceptionally large (greater than 100 Terabyte and often in the Petabyte and Exabyte 
range). In warehousing and analytic solutions, very large volumes of data pose challenges to data loading, 
modeling, cleansing, and analytics. These challenges are often solved using massively parallel processing, or 
 

