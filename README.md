ElasticSearch stores data as docs.

**Docs are stored under indexes**

# Cluster, Nodes, Shards and Replicas
Elasticsearch runs as a node inside a CLuster. Each cluster can have any number of node.
The reason to shard is to break the large amount of data into several nodes.

Example
We can decrease the query processing time drasticall from even 10 sec to 1 sec.
if a Single Shard in a Node contains 500K docs and it takes 10 sec to process a query
We can split that data into 10 nodes, so each node will have 50K docs.
Now it will take us only 1 sec to process 500K docs.

## Replicas
Replicas of a Shard are used to 
- Pevent downtime of a node
- If the Primary shrad is busy the Replica can be used to process the query
https://github.com/LisaHJung/Part-1-Intro-to-Elasticsearch-and-Kibana
