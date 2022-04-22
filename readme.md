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
=> A webhook is an HTTP request, triggered by an event in a source system and sent to a destination system, often with a payload of data. Webhooks are automated, in other words they are automatically sent out when their event is fired in the source system.

This provides a way for one system (the source) to "speak" (HTTP request) to another system (the destination) when an event occurs, and share information (request payload) about the event that occurred.

# What is Docker? Why do we use it?
=> Docker is an open source containerization platform. It enables developers to package applications into containers—standardized executable components combining application source code with the operating system (OS) libraries and dependencies required to run that code in any environment.

# What is S3 Service in AWS?
=> An Amazon S3 bucket is a public cloud storage resource available in Amazon Web Services' (AWS) Simple Storage Service (S3), an object storage offering. Amazon S3 buckets, which are similar to file folders, store objects, which consist of data and its descriptive metadata.

OR

Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. Customers of all sizes and industries can use Amazon S3 to store and protect any amount of data for a range of use cases, such as data lakes, websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics. Amazon S3 provides management features so that you can optimize, organize, and configure access to your data to meet your specific business, organizational, and compliance requirements.

# What is EC2 Instance in AWS?
=> An Amazon EC2 instance is a virtual server in Amazon's Elastic Compute Cloud (EC2) for running applications on the Amazon Web Services (AWS) infrastructure.

OR

Amazon Elastic Compute Cloud (Amazon EC2) provides scalable computing capacity in the Amazon Web Services (AWS) Cloud. Using Amazon EC2 eliminates your need to invest in hardware up front, so you can develop and deploy applications faster. You can use Amazon EC2 to launch as many or as few virtual servers as you need, configure security and networking, and manage storage. Amazon EC2 enables you to scale up or down to handle changes in requirements or spikes in popularity, reducing your need to forecast traffic.

# What is Cloudfront in AWS?
=> Amazon CloudFront is a web service that speeds up distribution of your static and dynamic web content, such as . html, . css, . js, and image files, to your users. CloudFront delivers your content through a worldwide network of data centers called edge locations.

# What is Route 53 In AWS?
=> Amazon Route 53 is a highly available and scalable Domain Name System (DNS) web service. You can use Route 53 to perform three main functions in any combination: domain registration, DNS routing, and health checking.

# What are ELBs in AWS?
=> Elastic Load Balancing (ELB) automatically distributes incoming application traffic across multiple targets and virtual appliances in one or more Availability Zones (AZs).

# What is TLS?
=> TLS Basics. Transport Layer Security (TLS) encrypts data sent over the Internet to ensure that eavesdroppers and hackers are unable to see what you transmit which is particularly useful for private and sensitive information such as passwords, credit card numbers, and personal correspondence.

# What is the difference HTTPS vs HTTP?
=> HTTPS is HTTP with encryption. The only difference between the two protocols is that HTTPS uses TLS (SSL) to encrypt normal HTTP requests and responses. As a result, HTTPS is far more secure than HTTP. A website that uses HTTP has http:// in its URL, while a website that uses HTTPS has https://.

# What is a reverse proxy?
=> A reverse proxy is a server that sits in front of web servers and forwards client (e.g. web browser) requests to those web servers. Reverse proxies are typically implemented to help increase security, performance, and reliability. In order to better understand how a reverse proxy works and the benefits it can provide, let’s first define what a proxy server is.
