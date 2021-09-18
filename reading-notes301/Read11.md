# SQL database and noSQL database
##  SQL database
A SQL database supports structured query language (SQL) — a domain-specific programming language for querying and manipulating data in a relational database. The key to the relational model is abstracting data as a set of tuples organized into “relations,” which allows for abstraction over the physical representation of data and access paths.

The "relational" in “relational database” refers to the "relational model" of data management devised by IBM researcher E.F. Codd in the early 1970s. Though SQL is not the only language used for implementing query over the relational model, it is the most popular (despite not strictly conforming to Codd's original design). Beginning with “System R,” the relational model was later popularized by subsequent database systems.

Relational databases have been the industry standard since the late 1970s, though many of their "navigational" predecessors (e.g., Apollo 11-era IMS) are still under active development. In fact, most current enterprise systems architecturally descend from the aforementioned System R.
## NoSQL database
Rooted in graph, document, key-value pairs and wide-column stores developed in the early 1990’s, NoSQL (“Not only SQL”) rose in the mid-2000s due to the emergence of cloud, big data, and web and mobile applications. Today it is the preferred database due to its performance quality, ability to scale and ease of use.

Research on non-relational systems (e.g., BigTable and Dynamo) led to the rise of startups and open source projects dedicated to increasing the relational model’s horizontal scalability and loosening the rigidity of its table design. Their emergence revealed a need for better designs and looser constraints for relational databases.

Though the relational database community responded to these needs with NewSQL, new databases continued to rapidly appear. As a result, multiple database systems now exist, each addressing the fundamental problem (i.e., storing bits and making them available later) in a slightly different way.

In many ways, this boom is a boon for developers. Not all applications have relational database-shaped problems or need to make the tradeoffs that relational databases impose on data and availability models. However, this flexibility does not come without a cost.

To make a good technical decision between NoSQL databases, a developer must have a thorough understanding of the full design space so the tradeoffs made by a particular system are clear. In other words, you don't want to accidentally sacrifice consistency isolation when your application actually requires it.

## SQL vs NoSQL: High-Level Differences

1. SQL databases are primarily called as Relational Databases (RDBMS); whereas NoSQL database are primarily called as non-relational or distributed database.
2. SQL databases are table based databases whereas NoSQL databases are document based, key-value pairs, graph databases or wide-column stores. This means that SQL databases represent data in form of tables which consists of n number of rows of data whereas NoSQL databases are the collection of key-value pair, documents, graph databases or wide-column stores which do not have standard schema definitions which it needs to adhered to.
3. SQL databases have predefined schema whereas NoSQL databases have dynamic schema for unstructured data.
4. SQL databases are vertically scalable whereas the NoSQL databases are horizontally scalable. SQL databases are scaled by increasing the horse-power of the hardware. NoSQL databases are scaled by increasing the databases servers in the pool of resources to reduce the load.
