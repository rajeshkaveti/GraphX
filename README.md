# GraphX


Apache Spark is a distributed computing system for large scale processing and is growing in popularity due to its speed. Apache Spark libraries has support for SPARK SQL and MLIB for machine learning. In addition, it also supports GraphX which is the graph processing layer on top of Spark bringing the power of Big Data processing to graphs. The library offers tools and techniques that can be used to mine APIs for PageRank, Topic Modeling, Graph Subsets, Shortest distances etc.

This project is primarily a Jupyter notebook demonstrating SPARK API for GRAPHX.  The example is based on Databricks example which uses 2 sets of data – Airline Performance and Airport data. The flights form the edges and airports are essentially vertices or nodes.

GraphX is still in the early stages. It is currently supported in SCALA and extends the RDD in SPARK by introducing the Resilient Distributed Property Graph on top of it.  For Python, a new set of API is being developed but it is still in the early stages. Jupyter notebooks has a strong ecosystem in Python and I would like to leverage some of the capabilities around visualization.

Databricks released Python based GraphFrames in March 2016. GraphFrames is based on DataFrame opening the ease and convenience of using SPARK SQL instead of using relatively complex RDD. 

In this project, I have used DataFrame based Graphs on top of Apache Spark providing me the convenience of writing SQL friendly queries. It provides performance benefits of DataFrame performance along with using PANDAS API. It also has visualization capabilities of MATPLOTLIB and other user-friendly libraries.

This example uses the same data that is used in DataBricks [Blog] (https://databricks.com/blog/2016/03/16/on-time-flight-performance-with-graphframes-for-apache-spark.html)., I also used "Learning PySpark" book leveraging some code snippets.
GraphX does not have any visualization component. Vendor products for instance NEO4J have good user capabilities around visualization. I have shown the usage of those products to enhance the visualization.
<br>
The example below uses the flight and airport data to illustrate some of the strengths of graph database. Some of the questions like 
•	Airport that is the busiest?
•	Which is the most important airport? (PageRank)
•	Which Airport causes the most delay?
•	When to expect delay when flying from a location?
•	Which flight are generally late when flying into a destination?

The data that I had originally used was larger. Due to limitation in GITHUB, I loaded a smaller version of the file

[Setup Up ](https://www.youtube.com/watch?v=uJeY3WRZGfw)

[Graph Notebook](https://github.com/rajeshkaveti/GraphX/blob/master/graphframev3.ipynb)
