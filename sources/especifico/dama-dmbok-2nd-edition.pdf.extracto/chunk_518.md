# página 519 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

BIG DATA AND DATA SCIENCE • 515 
example, customer purchase history would be needed to pre-populate a retail market-basket recommendation 
model. In predicting behavior of retail markets, historical price and price change information are combined with 
customer, demographic, and weather information. 
2.6.2 Train the Model 
Execute the model against the data in order to ‘train’ the model. Training includes repeated runs of the model 
against the data to verify assumptions. Training will result in changes to the model. Training requires balance. 
Avoid over-fitting by training against a limited data fold.  
Model validation must be complete before transitioning to production. Address any population imbalances or 
data biases with model offsets that are trained and validated; this can be tweaked in production as the initial 
offset is gradually adjusted through actual population interactions. Optimizing feature mix can be accomplished 
with Bayesian co-selection, classifier inversion, or rule induction. Models can also be combined for ensemble 
learning where the predictor model is built by combining the collected strengths of simpler models.  
Identifying outliers or anomalies (data objects that do not comply with the general behavior exhibited by the 
studied elements) is critical to the evaluating the model. For more volatile datasets, apply a variance test based 
on the average and standard deviation. Both tests can be readily applied on profiled results. It may be that the 
outliers are the target of the exercise, as opposed to finding and validating trends in the majority of the data. 
For predictive analytics, use a real-time data stream to finish the population of the predictive model and trigger 
a response, which might be an alert or an event. The data stream may require special focus on design and 
development of an extreme low latency processing capability. In some models, the difference in value of the 
predictions between fractions of a second is extreme and solutions may require innovative technology with 
speed of light limitations. 
Models can use many statistical functions and techniques that are available in open source libraries, one of 
which is ‘R.’ The R Project for Statistical Computing is a free software environment for statistical computing; it 
contains many functions as service calls.94 Custom functions can be developed leveraging the scripting 
language and shared across tools, platforms, and organizations.  
Once the solution design has been created and development and operation estimated, the organization may 
decide whether to develop the solution to predict behavior. Real-time operational analytics solutions frequently 
require substantial amounts of new architecture and development and could possibly not be cost effective. 
2.6.3 Evaluate Model 
Once the data is placed onto a platform and ready for analysis, the Data Science begins. The model is 
constructed, evaluated against training sets, and validated. Refinements to the business requirements are 
94 For more information, visit the R-Project website: http://bit.ly/19WExR5. 
 

