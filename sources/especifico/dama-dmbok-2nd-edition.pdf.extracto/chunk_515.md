# página 516 — de Dama-dmbok-data-management-body-of-knowledge-2nd-edition.pdf

512 • DMBOK2 
•
The timeliness and scope of the data to provision: Many elements can be provided in real-time
feeds, snapshots at a point in time, or even integrated and summarized. Low latency data is ideal, but
often comes at the expense of machine learning capabilities – there is a huge difference between
computational algorithms directed to data-at-rest versus streaming. Do not minimize the level of
integration required for downstream usage.
•
The impact on and relation to other data structures: There may need to be structure or content
changes in other data structures to make them suitable for integration with Big Data sets.
•
Influences to existing modeled data: Including extending the knowledge on customers, products, and
marketing approaches.
The strategy will drive the scope and timing of an organization’s Big Data capability roadmap. 
2.2 Choose Data Sources 
As with any development project, the choice of data sources for Data Science work must be driven by the 
problems the organization is trying to solve. The difference with Big Data / Data Science development is that 
the range of data sources is wider. It is not limited by format and can include data both external to and internal 
to an organization. The ability to incorporate this data into a solution also comes with risks. The quality and 
reliability of the data needs to be evaluated and a plan for use over time needs to be put into place. Big Data 
environments make it possible to quickly ingest lots of data, but to use that data and manage it over time, it is 
still necessary to know basic facts: 
•
Its origin
•
Its format
•
What the data elements represent
•
How it connects to other data
•
How frequently it will be updated
As more data becomes available (like US Census Bureau Statistics, shopping demographics, weather satellite 
data, research data sets), data needs to be evaluated for worth and reliability. Review the available data sources, 
and the processes that create those sources and manage the plan for new sources.  
•
Foundational data: Consider foundational data components such as POS (Point of Sale) in a sales
analysis.
•
Granularity: Ideally, obtain data in its most granular form (not aggregated). That way it can be
aggregated for a range of purposes.
•
Consistency: If possible, select data that will appear appropriately and consistently across
visualizations, or recognize limitations.
•
Reliability: Choose data sources that are meaningful and credible over time. Use trusted, authoritative
sources.
•
Inspect/profile new sources: Test changes before adding new data sets. Unexpected material or
significant changes in visualization outcomes can occur with the inclusion of new data sources.
 

