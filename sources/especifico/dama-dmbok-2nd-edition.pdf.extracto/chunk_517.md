# página 518 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

514 • DMBOK2 
2.4 Develop Data Hypotheses and Methods 
Data Science is about building answer sets that can find meaning or insights within the data. The development 
of Data Science solutions entails building statistical models that find correlations and trends within and between 
data elements and data sets. There will be multiple answers to a question based upon inputs to a model. For 
example, one must choose a rate of return to calculate the future value of a financial portfolio. Models often 
have more than one variable so the best practice is to find deterministic outcomes – or in other words, use best 
guesses as to the values to be expected. However, best guesses themselves should be educated. Each model will 
operate depending on the analysis method chosen. It should be tested for a range of outcomes, even the ones 
that appear least probable.  
Models depend on both the quality of input data and the soundness of the model itself. Data models can often 
give insight into how to correlate the information found. An example of this is using K-Means clustering to 
determine the number of groupings of data to analyze further. (See Chapter 13.) 
2.5 Integrate / Align Data for Analysis 
Preparing the data for analysis involves understanding what is in the data, finding links between data from the 
various sources, and aligning common data for use.  
In many cases, joining data sources is more an art than a science. For example, consider one data set based upon 
daily updates and another based upon monthly updates. The daily data, in order to be aligned, would have to be 
aggregated so that there would be an alignment pattern that could be used in the Data Science investigation. 
One method is to use a common model that integrates the data using a common key. Another way is to scan and 
join data using indexes within the database engines for similarity and record linkage algorithms and methods. 
Often data is inspected during the initial phases to understand how the data could be analyzed. Clustering helps 
determine the grouping of the data outputs. Other methods can find correlations that will be used to build the 
model to display results. Consider using techniques during the initial phases that will aide in understanding how 
the model will show results once published. 
Most solutions require the integration of Master Data and Reference Data in order to interpret results of the 
analytics. (See Chapter 10.) 
2.6 Explore Data Using Models 
2.6.1 Populate Predictive Model 
Configuring predictive models includes pre-populating the model with historical information concerning the 
customer, market, products, or other factors that are included in the model other than the triggering factor. Pre-
population calculations are usually performed in advance to enable the fastest response to triggering events. For 
 

