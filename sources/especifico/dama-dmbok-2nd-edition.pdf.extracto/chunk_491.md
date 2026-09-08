# página 492 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

488 • DMBOK2 
•
Measurability: A data quality metric must be measurable – it needs to be something that can be
counted. For example, data relevancy is not measurable, unless clear criteria are set for what makes
data relevant. Even data completeness needs to be objectively defined in order to be measured.
Expected results should be quantifiable within a discrete range.
•
Business relevance: While many things are measurable, not all translate into useful metrics.
Measurements need to be relevant to data consumers. The value of the metric is limited if it cannot be
related to some aspect of business operations or performance. Every data quality metric should
correlate with the influence of the data on key business expectations.
•
Acceptability: The data quality dimensions frame the business requirements for data quality.
Quantifying along the identified dimension provides hard evidence of data quality levels. Determine
whether data meets business expectations based on specified acceptability thresholds. If the score is
equal to or exceeds the threshold, the quality of the data meets business expectations. If the score is
below the threshold, it does not.
•
Accountability / Stewardship: Metrics should be understood and approved by key stakeholders (e.g.,
business owners and Data Stewards). They are notified when the measurement for the metric shows
that the quality does not meet expectations. The business data owner is accountable, while a data
steward takes appropriate corrective action.
•
Controllability: A metric should reflect a controllable aspect of the business. In other words, if the
metric is out of range, it should trigger action to improve the data. If there is no way to respond, then
the metric is probably not useful.
•
Trending: Metrics enable an organization to measure data quality improvement over time. Tracking
helps Data Quality team members monitor activities within the scope of a data quality SLA and data
sharing agreement, and demonstrate the effectiveness of improvement activities. Once an information
process is stable, statistical process control techniques can be applied to detect changes to the
predictability of the measurement results and the business and technical processes on which it provides
insight.
4.5 Statistical Process Control 
Statistical Process Control (SPC) is a method to manage processes by analyzing measurements of variation in 
process inputs, outputs, or steps. The technique was developed in the manufacturing sector in the 1920s and has 
been applied in other industries, in improvement methodologies such as Six Sigma, and in Data Quality 
Management.87 Simply defined, a process is a series of steps executed to turn inputs into outputs. SPC is based 
on the assumption that when a process with consistent inputs is executed consistently, it will produce consistent 
outputs. It uses measures of central tendency (how values cluster around a central value, such as a mean, 
87 See Redman (1996 and 2001), Loshin (2000), Sebastian-Coleman (2013), Jugulum (2014). 
 

