# página 526 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

522 • DMBOK2 
its purpose is different. It does not predict outcomes; it seeks to match model results only with existing 
data.  
Key to predictive analytics is to learn by example through training the model. Performance of a learning method 
relates its predictive abilities on independent test data. Assessment guides the choice of learning and measures 
the quality of the chosen model. Model selection estimates performance where assessment evaluates the 
generalization error on new data.  
Avoid over-fitting – a situation that occurs when the model is trained against non-representative datasets, is 
overly complex in relation to its data, or has described noise instead of the underlying relationship(s). Use 
additional techniques such as K-fold validation to indicate when training is no longer resulting in better 
generalization. 
Training error consistently decrease with model complexity and can drop off to zero. Therefore, it is not a 
useful estimate of the test error. Randomly divide the data set into three parts to form training, testing, and 
validation sets. The training set is used to fit the model, the validation set is used to predict error for selection, 
and the test set is used for assessment of the generalization error of the final model.  
Reusing the same test-set repeatedly can underestimate the true test error. Ideally, perform cross-validation by 
randomly dividing the data set into a set of K-folds or cross-validation groups. Perform training on all but one 
set of data based on strongly correlated predictor variables. Test the model on the remaining piece and 
determine generalization error based on all K-folds. Several statistical tests can be applied and performed to 
numerically assess contextual model validity.  
4.2 Big Data Modeling 
Modeling Big Data is a technical challenge but critical if an organization that wants to describe and govern its 
data. Traditional Enterprise Data Architecture principles do apply; data needs to be integrated, specified, and 
managed.  
The main driver to physically model a data warehouse is to enable population of data for query performance. 
This driver is not in play for Big Data. This is not an excuse to abandon the modeling process or to hand it off to 
a developer. The value of modeling the data is that it enables people to understand data content. Apply proven 
data modeling techniques while accounting for the variety of sources. Develop the subject area model, at least 
in a summarized way, so it can be related to proper contextual entities and placed into the overall roadmap, just 
like any other kind of data. The challenge is to make an understandable and useful picture out of these large 
data sets, and for a justifiable cost.  
Understand how the data links between data sets. For data of different granularity, prevent combinations that 
count data elements or values more than once; for example, don’t combine atomic and aggregate sets. 
 

