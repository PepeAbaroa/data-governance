# página 168 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

164 • DMBOK2 
a change affects the logical data model, such as a new or changed business data requirement, the data analyst or 
architect must review and approve the change to the model. 
Each change should note: 
•
Why the project or situation required the change
•
What and How the object(s) changed, including which tables had columns added, modified, or
removed, etc.
•
When the change was approved and when the change was made to the model (not necessarily when
the change was implemented in a system)
•
Who made the change
•
Where the change was made (in which models)
Some data modeling tools include repositories that provide data model versioning and integration functionality. 
Otherwise, preserve data models in DDL exports or XML files, checking them in and out of a standard source 
code management system just like application code. 
5.2 Data Modeling Metrics 
There are several ways of measuring a data model’s quality, and all require a standard for comparison. One 
method that will be used to provide an example of data model validation is The Data Model Scorecard®, which 
provides 11 data model quality metrics: one for each of ten categories that make up the Scorecard and an overall 
score across all ten categories (Hoberman, 2015). Table 11 contains the Scorecard template.  
Table 11 Data Model Scorecard® Template 
# 
Category 
Total 
score 
Model 
score 
% 
Comments 
1 
How well does the model capture the requirements? 
15 
2 
How complete is the model? 
15 
3 
How well does the model match its scheme? 
10 
4 
How structurally sound is the model? 
15 
5 
How well does the model leverage generic structures? 
10 
6 
How well does the model follow naming standards? 
5 
7 
How well has the model been arranged for 
readability? 
5 
8 
How good are the definitions? 
10 
9 
How consistent is the model with the enterprise? 
5 
10 
How well does the metadata match the data? 
10 
TOTAL SCORE 
100 
The model score column contains the reviewer’s assessment of how well a particular model met the scoring 
criteria, with a maximum score being the value that appears in the total score column. For example, a reviewer 
might give a model a score of 10 on “How well does the model capture the requirements?” The % column 
 

