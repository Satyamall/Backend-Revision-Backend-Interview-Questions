Backend Interview Questions

# What is Caching? How can you save money with Caching?
=> In computing, a cache is a high-speed data storage layer which stores a subset of data, typically transient in nature, so that future requests for that data are served up faster than is possible by accessing the data’s primary storage location. Caching allows you to efficiently reuse previously retrieved or computed data.

The data in a cache is generally stored in fast access hardware such as RAM (Random-access memory) and may also be used in correlation with a software component. A cache's primary purpose is to increase data retrieval performance by reducing the need to access the underlying slower storage layer.

Trading off capacity for speed, a cache typically stores a subset of data transiently, in contrast to databases whose data is usually complete and durable.

# What is load balancing?
=> Load balancing is a core networking solution used to distribute traffic across multiple servers in a server farm. Load balancers improve application availability and responsiveness and prevent server overload.

# What is CAP Theorem?
=> The CAP theorem applies a similar type of logic to distributed systems—namely, that a distributed system can deliver only two of three desired characteristics: consistency, availability, and partition tolerance (the ‘C,’ ‘A’ and ‘P’ in CAP).

A distributed system is a network that stores data on more than one node (physical or virtual machines) at the same time. Because all cloud applications are distributed systems, it’s essential to understand the CAP theorem when designing a cloud app so that you can choose a data management system that delivers the characteristics your application needs most.

# What is PACELC Theorem?
=> The PACELC theorem states that in a system that replicates data:
- if there is a partition (‘P’), a distributed system can tradeoff between availability and consistency (i.e., ‘A’ and ‘C’);
- else (‘E’), when the system is running normally in the absence of partitions, the system can tradeoff between latency (‘L’) and consistency (‘C’).

The first part of the theorem (PAC) is the same as the CAP theorem, and the ELC is the extension. The whole thesis assumes we maintain high availability by replication. So, when there is a failure, CAP theorem prevails. But if not, we still have to consider the tradeoff between consistency and latency of a replicated system.

# What is Eventual Consistency?
=> Eventual Consistency is a guarantee that when an update is made in a distributed database, that update will eventually be reflected in all nodes that store the data, resulting in the same response every time the data is queried.

# What is Strong Consistency?
=> Strong consistency is one of the consistency models used in the domain of concurrent programming (e.g., in distributed shared memory, distributed transactions). The protocol is said to support strong consistency if: All accesses are seen by all parallel processes (or nodes, processors, etc.)

# What are the different types of databases?
=> There are following types of databases are: 
 - Centralised database.
 - Distributed database.
 - Personal database.
 - End-user database.
 - Commercial database.
 - NoSQL database.
 - Operational database.
 - Relational database.
 - Cloud database.
 - Object-oriented database.
 - Graph database.

# What are message queues?
=> A message queue is a form of asynchronous service-to-service communication used in serverless and microservices architectures. Messages are stored on the queue until they are processed and deleted. Each message is processed only once, by a single consumer. Message queues can be used to decouple heavyweight processing, to buffer or batch work, and to smooth spiky workloads.

# Which service by Amazon Web Services (AWS) can you use for Queues?
=> Amazon Simple Queue Service (SQS) is a fully managed message queuing service that enables you to decouple and scale microservices, distributed systems, and serverless applications.

# What is Pub Sub ?
=> Publish/subscribe messaging, or pub/sub messaging, is a form of asynchronous service-to-service communication used in serverless and microservices architectures. In a pub/sub model, any message published to a topic is immediately received by all of the subscribers to the topic.

# How do you go about sending a million emails? What are the steps you will take to ensure system is stable, and will end up with lesser failures?
=> Well, first of all it should be clear to you that you cannot use a common mail client or a webmail. Opening up your Gmail account and importing all the million contacts in the BCC line would be crazy – and impossible, because a normal email provider gives you only a limited number of relays per day.

Also, these providers use non-monitored SMTP servers that strictly depend on your internet connection at the given moment and can rely on bad IPs which can harm your deliverability.

So to send 1 million (or also 1000, or 10.000, or no matter how many) good emails you need first of all a reliable, effective bulk email service or software able to manage a wide list. But you also need a professional SMTP provider like turboSMTP, in order to ensure the highest delivery rate of your emails.

Eight Ways to Achieve System Stability
 - Define (Your) System Stability. ...
 - Create Change Management Policies. ...
 - Enforce End-to-End Test Procedures. ...
 - Map and Monitor Your Network. ...
 - Proper Server Monitoring. ...
 - Implement Corporate Collaboration Tools. ...
 - Test System Restoration Procedures. ...
 - Use Big Data Analytics to Predict Outages.

# What are webhooks? 
=> 