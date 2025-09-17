# 📘 System Design Mock Interview – 50 MCQs with Answers & Explanations

Welcome to the **System Design Mock Interview Guide** 🎯  
This file contains **50 beginner-to-advanced MCQs** on System Design, complete with **correct answers and explanations**.  
Use it to revise concepts, understand trade-offs, and practice interview-style questions.  

---

## Structure
Each question is followed by:
1. Options (MCQ format)  
2. Correct Answer
3. Explanation  

---

## 📂 Questions

### Question 1  
**What is Vertical Scaling?**  
A. Adding more machines to your system  
B. Adding more CPUs/RAM to an existing machine  
C. Distributing traffic across multiple servers  
D. Using CDN for faster delivery  

**Answer:** B  
**Explanation:** Vertical scaling means improving the capacity of a single machine by adding more CPU, RAM, or storage.  

---

### Question 2  
**What is Horizontal Scaling?**  
A. Increasing RAM in one server  
B. Adding more servers to handle load  
C. Caching results for faster response  
D. Optimizing database queries  

**Answer:** B  
**Explanation:** Horizontal scaling involves adding more servers to distribute traffic and workload.  

---

### Question 3  
**In a load balancer setup, which strategy distributes traffic evenly without considering server load?**  
A. Least connections  
B. Round Robin  
C. Weighted round robin  
D. Random  

**Answer:** B  
**Explanation:** Round Robin rotates requests evenly across servers, without checking load.  

---

### Question 4  
**Which is an example of a CDN (Content Delivery Network)?**  
A. Redis  
B. Akamai  
C. PostgreSQL  
D. RabbitMQ  

**Answer:** B  
**Explanation:** Akamai, Cloudflare, AWS CloudFront are CDNs for caching static/dynamic content near users.  

---

### Question 5  
**Which database is best suited for storing social network connections (friend graph)?**  
A. Relational DB  
B. Graph DB (like Neo4j)  
C. Time-series DB  
D. Key-value DB  

**Answer:** B  
**Explanation:** Graph databases are optimized for relationships like friends/followers.  

---

### Question 6  
**What is a CAP theorem tradeoff in distributed systems?**  
A. Consistency, Availability, Partition Tolerance (only 2 at once)  
B. CPU, Availability, Performance  
C. Cache, Access, Partitioning  
D. Cost, Accuracy, Performance  

**Answer:** A  
**Explanation:** CAP theorem states a distributed system can guarantee only two of Consistency, Availability, Partition tolerance.  

---

### Question 7  
**Which caching strategy ensures data is loaded into cache only when requested?**  
A. Write-through cache  
B. Read-through cache  
C. Write-around cache  
D. Refresh-ahead cache  

**Answer:** B  
**Explanation:** Read-through loads data into cache when a request misses.  

---

### Question 8  
**What’s the biggest drawback of vertical scaling?**  
A. Complexity of sharding  
B. Hardware limits and single point of failure  
C. High latency across servers  
D. Requires CDN integration  

**Answer:** B  
**Explanation:** Vertical scaling is limited by hardware max specs and introduces a single point of failure.  

---

### Question 9  
**Why do companies like Netflix use microservices instead of monoliths?**  
A. To save disk space  
B. To independently scale and deploy services  
C. To avoid using databases  
D. To eliminate network calls  

**Answer:** B  
**Explanation:** Microservices allow independent deployment, scaling, and fault isolation.  

---

### Question 10  
**Which database model fits for IoT sensor data (time-ordered logs)?**  
A. Key-value store  
B. Document DB  
C. Time-series DB  
D. Graph DB  

**Answer:** C  
**Explanation:** Time-series DBs are designed for sequential, timestamped data like metrics and IoT sensors.  

---

### Question 11  
**In system design, what is a CDN primarily used for?**  
A. Reducing database load  
B. Delivering content closer to users  
C. Storing logs  
D. Managing pub-sub messaging  

**Answer:** B  
**Explanation:** CDNs reduce latency by caching data geographically closer to users.  

---

### Question 12  
**Which type of database is DynamoDB?**  
A. Relational DB  
B. Key-value / Document store (NoSQL)  
C. Graph DB  
D. In-memory DB  

**Answer:** B  
**Explanation:** DynamoDB is a NoSQL key-value/document database.  

---

### Question 13  
**Which partitioning strategy assigns data to servers using a hash function?**  
A. Range partitioning  
B. Hash partitioning  
C. Directory-based partitioning  
D. Round robin  

**Answer:** B  
**Explanation:** Hash partitioning uses hash functions to map data to nodes.  

---

### Question 14  
**Which service is an example of managed message queues?**  
A. AWS SQS  
B. Redis Cache  
C. MySQL Replication  
D. Cloudflare CDN  

**Answer:** A  
**Explanation:** AWS SQS, RabbitMQ, Kafka are message queues for async processing.  

---

### Question 15  
**What’s the role of a load balancer in system design?**  
A. Cache static content  
B. Distribute traffic among servers  
C. Store logs  
D. Replace databases  

**Answer:** B  
**Explanation:** Load balancers distribute incoming traffic across multiple servers for performance & fault tolerance.  

---

### Question 16  
**Which consistency model ensures all reads reflect the most recent write?**  
A. Strong consistency  
B. Eventual consistency  
C. Causal consistency  
D. Weak consistency  

**Answer:** A  
**Explanation:** Strong consistency ensures reads always see the latest write.  

---

### Question 17  
**What’s a drawback of eventual consistency?**  
A. Always slower response times  
B. Reads may see stale data  
C. Requires sharding  
D. Impossible to scale  

**Answer:** B  
**Explanation:** Eventual consistency allows stale reads until replicas catch up.  

---

### Question 18  
**Which company popularized Chaos Engineering to test resilience?**  
A. Twitter  
B. Netflix  
C. Facebook  
D. Google  

**Answer:** B  
**Explanation:** Netflix developed Chaos Monkey to test failure handling in production.  

---

### Question 19  
**What is rate limiting used for?**  
A. To prevent a single user/system from overloading services  
B. To speed up responses  
C. To shard databases  
D. To enforce strong consistency  

**Answer:** A  
**Explanation:** Rate limiting protects APIs/systems from abuse and excessive traffic.  

---

### Question 20  
**Which database is suitable for flexible JSON-like storage?**  
A. MySQL  
B. MongoDB  
C. Cassandra  
D. Neo4j  

**Answer:** B  
**Explanation:** MongoDB is a document DB optimized for JSON-like storage.  

---

### Question 21  
**What is a write-ahead log (WAL) used for in databases?**  
A. Caching reads  
B. Ensuring durability by writing logs before applying changes  
C. Speeding up queries  
D. Load balancing  

**Answer:** B  
**Explanation:** WAL ensures durability; changes are logged before being applied.  

---

### Question 22  
**What is the purpose of a reverse proxy like NGINX?**  
A. Serve as a CDN  
B. Handle client requests, load balance, cache, and SSL termination  
C. Partition databases  
D. Manage transactions  

**Answer:** B  
**Explanation:** Reverse proxies add caching, load balancing, and SSL offloading.  

---

### Question 23  
**Which storage type is best for high availability and redundancy?**  
A. Local disk  
B. RAID 0  
C. Distributed file system (HDFS, S3)  
D. Temporary cache  

**Answer:** C  
**Explanation:** Distributed file systems replicate data across nodes for availability.  

---

### Question 24  
**Which hashing technique reduces reassignments when scaling clusters?**  
A. Simple modulo hashing  
B. Consistent hashing  
C. Range hashing  
D. Directory hashing  

**Answer:** B  
**Explanation:** Consistent hashing minimizes key remapping when nodes are added/removed.  

---

### Question 25  
**What’s the role of ZooKeeper in distributed systems?**  
A. Store documents  
B. Provide coordination, leader election, config management  
C. Cache static content  
D. Enforce strong consistency  

**Answer:** B  
**Explanation:** ZooKeeper is used for coordination and metadata management.  

---

### Question 26  
**What’s the main drawback of synchronous replication?**  
A. Data loss  
B. High latency due to waiting for all replicas  
C. Lower durability  
D. Poor consistency  

**Answer:** B  
**Explanation:** Sync replication adds latency since writes wait for acknowledgments.  

---

### Question 27  
**What’s the purpose of sharding in databases?**  
A. Store backups  
B. Distribute data across nodes for scalability  
C. Increase consistency  
D. Speed up queries always  

**Answer:** B  
**Explanation:** Sharding splits data across nodes to handle scale.  

---

### Question 28  
**Which design ensures services remain available if one data center goes down?**  
A. Vertical scaling  
B. Multi-region active-active deployment  
C. Caching  
D. Event sourcing  

**Answer:** B  
**Explanation:** Active-active deployments ensure redundancy across regions.  

---

### Question 29  
**Which approach allows search engines like Google to quickly look up documents?**  
A. B-trees  
B. Inverted indexes  
C. Bloom filters  
D. Skip lists  

**Answer:** B  
**Explanation:** Inverted indexes map words → documents for fast search.  

---

### Question 30  
**Why use Bloom Filters in large systems (e.g., databases, caching)?**  
A. To compress logs  
B. To quickly test set membership with low memory  
C. To replace indexes  
D. To sort data  

**Answer:** B  
**Explanation:** Bloom filters test membership quickly with minimal memory, though false positives exist.  

---

### Question 31  
**Which queue design handles retries & failure gracefully?**  
A. FIFO queue only  
B. Dead-letter queue  
C. Random queue  
D. Sticky sessions  

**Answer:** B  
**Explanation:** Dead-letter queues capture failed messages for later handling.  

---

### Question 32  
**Which approach avoids single point of failure in DB master-slave setups?**  
A. Single master  
B. Multi-master replication  
C. WAL logging  
D. Caching  

**Answer:** B  
**Explanation:** Multi-master allows multiple write nodes to prevent downtime.  

---

### Question 33  
**Which is an example of eventual consistency in real life?**  
A. ATM withdrawal updates instantly  
B. Facebook likes may appear after a few seconds  
C. Bank transfer across accounts instantly updates  
D. CDN always serves fresh data  

**Answer:** B  
**Explanation:** Likes/shares on social media propagate asynchronously = eventual consistency.  

---

### Question 34  
**Which database system does Amazon DynamoDB use principles from?**  
A. Google Bigtable  
B. Amazon Aurora  
C. Dynamo paper  
D. Oracle RAC  

**Answer:** C  
**Explanation:** DynamoDB is based on Amazon’s Dynamo system (Dynamo paper).  

---

### Question 35  
**What’s the purpose of circuit breaker pattern in microservices?**  
A. To shard databases  
B. To prevent cascading failures when a service is down  
C. To enforce strong consistency  
D. To reduce cache misses  

**Answer:** B  
**Explanation:** Circuit breaker halts calls to failing services to avoid chain failures.  

---

### Question 36  
**Which database is optimized for analytical queries (OLAP)?**  
A. MongoDB  
B. Cassandra  
C. Snowflake/Redshift  
D. MySQL  

**Answer:** C  
**Explanation:** Snowflake/Redshift are OLAP databases optimized for analytics.  

---

### Question 37  
**What’s the advantage of Quorum-based reads/writes (like in Cassandra)?**  
A. Always strong consistency  
B. Balance between consistency and availability  
C. Faster than caching  
D. Requires fewer replicas  

**Answer:** B  
**Explanation:** Quorum allows tuning consistency vs availability trade-offs.  

---

### Question 38  
**Which indexing method speeds up range queries (like time intervals)?**  
A. Hash index  
B. B-tree index  
C. Bitmap index  
D. Bloom filter  

**Answer:** B  
**Explanation:** B-trees are great for sorted range queries.  

---

### Question 39  
**Which is the best choice for sending millions of notifications reliably?**  
A. REST API only  
B. Message queue/broker (Kafka, RabbitMQ)  
C. File storage  
D. CDN  

**Answer:** B  
**Explanation:** Message brokers ensure reliability, retries, buffering.  

---

### Question 40  
**In high-traffic web apps, what’s the purpose of backpressure?**  
A. Improve queries with indexes  
B. Slow producers to avoid overwhelming consumers  
C. Compress logs  
D. Increase consistency  

**Answer:** B  
**Explanation:** Backpressure prevents overload by slowing producers if consumers lag.  

---

### Question 41  
**Which ID generation strategy is used by Twitter for unique IDs?**  
A. UUID v4  
B. Auto-increment IDs  
C. Snowflake ID generator  
D. Hash IDs  

**Answer:** C  
**Explanation:** Snowflake IDs encode timestamp + machine ID + sequence number.  

---

### Question 42  
**Which component is crucial in recommendation systems (like Netflix)?**  
A. Graph DB only  
B. Time-series DB  
C. Data lake / distributed storage  
D. CDN  

**Answer:** C  
**Explanation:** Data lakes store behavioral logs for ML recommendations.  

---

### Question 43  
**What’s the benefit of vector clocks?**  
A. Guarantee serializability  
B. Detect causality & ordering in distributed events  
C. Reduce bandwidth  
D. Speed consensus  

**Answer:** B  
**Explanation:** Vector clocks detect concurrency and ordering in distributed systems.  

---

### Question 44  
**Which strategy reroutes traffic if servers/data centers fail?**  
A. Sticky sessions  
B. Failover with health checks + DNS/load balancer updates  
C. Write-ahead logging  
D. Vertical scaling  

**Answer:** B  
**Explanation:** Failover ensures traffic is rerouted automatically during failures.  

---

### Question 45  
**Main advantage of event sourcing?**  
A. No need for DB  
B. Rebuild state by replaying events  
C. Zero latency  
D. Strict consistency  

**Answer:** B  
**Explanation:** Event sourcing records all changes as events, replayed to rebuild state.  

---

### Question 46  
**Why use caching hierarchy (browser → CDN → edge → origin)?**  
A. Reduce redundancy  
B. Reduce latency and server load progressively  
C. Replace load balancing  
D. Guarantee strong consistency  

**Answer:** B  
**Explanation:** Multi-layer caches progressively reduce latency/load.  

---

### Question 47  
**Which consistency model do social media feeds use?**  
A. Strong consistency  
B. Eventual consistency  
C. Linearizability  
D. Serializable  

**Answer:** B  
**Explanation:** Social feeds accept staleness for higher availability = eventual consistency.  

---

### Question 48  
**Why is Apache Kafka better than traditional queues for pipelines?**  
A. Guarantees serializability  
B. High throughput + durable log storage  
C. No need for DBs  
D. Zero latency  

**Answer:** B  
**Explanation:** Kafka handles massive throughput with durable logs.  

---

### Question 49  
**Why does Cassandra use gossip protocol?**  
A. Zero data loss  
B. Scalability & fault tolerance without single leader  
C. Faster queries than SQL  
D. Strong consistency  

**Answer:** B  
**Explanation:** Gossip protocol avoids single point of failure, enabling scale.  

---

### Question 50  
**What’s the role of a service mesh (Istio/Linkerd)?**  
A. Store logs  
B. Observability, security, traffic management between microservices  
C. Replace load balancers  
D. Shard databases  

**Answer:** B  
**Explanation:** Service meshes manage observability, security, and inter-service traffic.  

---
Thanks for going through this **System Design Mock Interview Guide**.  

