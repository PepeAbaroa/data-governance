# página 513 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

BIG DATA AND DATA SCIENCE • 509 
Frequently, the triggering factor is the accumulation of a large volume of real-time data, such as an extremely 
high number of trades or requests for service or volatility of the environment. Monitoring a data event stream 
includes incrementally building on the populated models until a threshold is reached as defined in the model. 
The amount of time that a predictive model provides between the prediction and event predicted is frequently 
very small (seconds or less than a second). Investment in very low latency technology solutions, such as in-
memory databases, high-speed networks, and even physically proximity to the source of the data, optimizes an 
organization’s ability to react to the prediction. 
The simplest form of predictive model is the forecast. Many techniques exist for trending or forecasting based 
on regression analysis and benefit from smoothing. The simplest way to smooth data is through a moving 
average, or even a weighted moving average. More advanced techniques can be useful, like the exponential 
moving average, which introduces a smoothing factor to be applied. Minimizing the error residual from the least 
squares can be a starting point, but several runs are necessary to determine and optimize the smoothing factor. 
Double and triple exponential smoothing models exist to address trend and seasonality components. 
1.3.12 Prescriptive Analytics 
Prescriptive analytics take predictive analytics a step farther to define actions that will affect outcomes, rather 
than just predicting the outcomes from actions that have occurred. Prescriptive analytics anticipates what will 
happen, when it will happen, and implies why it will happen. Because prescriptive analytics can show the 
implications of various decisions, it can suggest how to take advantage of an opportunity or avoid a risk. 
Prescriptive analytics can continually take in new data to re-predict and re-prescribe. This process can improve 
prediction accuracy and result in better prescriptions. 
1.3.13 Unstructured Data Analytics 
Unstructured data analytics combines text mining, association, clustering, and other unsupervised learning 
techniques to codify large data sets. Supervised learning techniques can also be applied to provide orientation, 
oversight, and guidance in the coding process leveraging human intervention to resolve ambiguity when 
necessary. 
Unstructured data analytics is becoming more important as more unstructured data is generated. Some analysis 
is impossible without the ability to incorporate unstructured data into analytical models. However, unstructured 
data is difficult to analyze without some way to isolate the elements of interest from extraneous elements.  
Scanning and tagging is one way to add ‘hooks’ to unstructured data that allow filtering and linking to related 
structured data. However, knowing what tags to generate based on what conditions is difficult. It is an iterative 
process, from when proposed tag conditions are identified, tags are assigned as data is ingested, then analytics 
uses those tags to validate the tag condition, and analyze the tagged data, which then leads to potentially 
changed tag conditions, or more tags.  
 

