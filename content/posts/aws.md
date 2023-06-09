---
title: "AWS"
date: 2023-06-02
showToc: true
TocOpen: false
draft: false
hidemeta: false
searchHidden: false
comments: false
disableHLJS: true # to disable highlightjs
disableShare: false
disableHLJS: true
hideSummary: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowWordCount: true
ShowRssButtonInSectionTermList: false
UseHugoToc: false
ShowPostNavLinks: false
---
{{< youtube JIbIYCM48to >}}

## Compute
AWS 5 main computing services 
1. Amazon Elastic Compute Cloud (EC2)
2. AWS Lambda
3. Amazon Elastic Container Service (ECS)
4. Amazon Elastic Kubernetes Service (EKS)
5. Amazon Elastic Beanstalk

*All of these services run on EC2 but are configured to certain needs.*

**EC2:**

- A virtual server where you can run applications and host services. 
- This is the most basic, flexible, and configurable service that Amazon provides. 
- Choose EC2 if AWS has no other service for your needs or if you want to manage your infrastructure 

**Lambda:**

- Event-driven computing service made for serverless applications
- You don't need to manage any servers. 
- Lets you write code in the form of *Lambda Functions* to perform a task in response to events.
- Known as a FaaS (Function as a Service)

**ECS:**

- A container orchestration service that supports Docker containers
- Has good integration with other AWS Services ( IAM, CloudWatch, ELB)
- More managed than EC2 but less complex than EKS
- Amazon's platform for cluster management infrastructure (like Kubernetes but simpler)

**EKS:**

- This is Amazon's managed Kubernetes service. Kubernetes is an open source container orchestration platform
- Great choice to avoid AWS lock-in which makes it great for a multi-cloud strategy
- makes it easy to run Kubernetes on AWS without needing to set up your own Kubernetes control plane or nodes.

**Elastic Beanstalk:**

- A platform as a service (PaaS) that makes it easy to create applications in multiple languages
- Automatically handles capacity provisioning, load balancing, and application health monitoring. 
- Easiest and simplest Solution
---

## Storage 
AWS 5 main storage services 

1. Amazon Simple Storage Service (S3)
2. Amazon Elastic Block Store (EBS)
3. Amazon Elastic File System (EFS)
4. Amazon Glacier
5. AWS Storage Gateway

*All of these services, except for Storage Gateway, run on S3 but are configured to certain needs.*


**S3:**

- A scalable object storage service for data archiving and backup.
- Can store any type of objects which includes data lakes, and/or big data analytics.
- S3 is often used as the data store for cloud-native applications, as well as for backups and big data projects.
- Data is organized into buckets and identified within each bucket by a unique, user-assigned key.
- Provides features like lifecycle management, encryption, and a robust permissions model.

**EBS:**

- A block storage service designed for use with Amazon EC2 instances.
- Particularly good for databases or any workload that requires frequent reads/writes to storage.
- Can be attached to an EC2 instance and used like a physical hard drive.


**EFS:**

- Managed file storage service that makes it easy to set up and scale file storage in the Amazon Cloud.
- EFS is designed to be used with EC2 instances, and multiple instances can connect to the system at once.
- Good for applications that require shared access to files and require a file system interface and file system semantics.

**Glacier:**

- A secure, durable, and low-cost storage service for data archiving and long-term backup.
- Designed to be really durable
- Used to move infrequently accessed data off to a low-cost storage service.

**Storage Gateway:**

- A hybrid cloud service that allows on-premises applications to access virtually unlimited cloud storage with the AWS cloud storage 
- Also good for local caching for low-latency access to hot data, then sync to AWS for durable storage.


---
## Database
AWS 5 main database services 
1. Amazon Relational Database Service (RDS)
2. Amazon DynamoDB
3. Amazon Redshift
4. Amazon ElastiCache
5. Amazon Neptune


**RDS:**

- Managed relational database service that supports several database engines (MySQL, PostgreSQL)
- Automatically takes care of routine database tasks 
- Suited for applications that require complex queries and transaction capabilities.

**DynamoDB:**

- A NoSQL database service for applications that need high-performance at any scale.
- Has built-in security, backup and restore, and in-memory caching for internet-scale applications
- Supports both key-value and document data models

**Redshift:**

- A fully managed, petabyte-scale data warehousing service.
- Used in conjunction with data analytics tools to allow analytical queries involving large datasets.
- It has fast query due to  columnar storage and parallel queries across multiple nodes 

**ElastiCache:**
- A fully managed in-memory data store service
- improves the speed of web applications by allowing you to retrieve information from fast, managed, in-memory caches
- Good for caching, session storage, gaming, geospatial services, real-time analytics, and queueing.


**Neptune:**

- A managed graph database service
- For applications that work with highly connected databases
- Could be used to create knowledge graphs, fraud detection systems, recommendation engines, etc. 

---
## Network
AWS 5 main network services 
1. Amazon Virtual Private Cloud (VPC)
2. Amazon Route 53
3. AWS Direct Connect
4. Elastic Load Balancer (ELB)
5. Amazon API Gateway


**VPC:**

- Provides an isolated virtual network where you can launch AWS resources to the AWS Cloud.
- You can define your own IP address range, create subnets, configure route tables, and network gateways.
- Has both IPv6 and IPv4 for most resources. 

**Route 53:**

- A  Domain Name System (DNS) web service.
- It's has domain registration, domain routing, and health checking of resources within your environment.
- It connects user requests to infrastructure running in AWS, like EC2 instances, or S3 buckets.
- Also has domain registration services that allows you to transfer or register domain names. 

**Direct Connect:**

- Establishes a dedicated network connection from your premises to AWS.
- In comparison to internet-based connections it can it reduces your network costs, increases bandwidth throughput, and provides just a more consistent network experience. 

**ELB:**

- A load balancer for AWS targets (EC2, Containers, IP addresses, Lambda functions)
- It ensures the delivery of the right amount of traffic to each target based on the capacity that you set.
- Has three different load balancers: Application Load Balancer, Network Load Balancer, and Classic Load Balancer.

**API Gateway:**

- A service for APIs.
- Handles all the tasks (traffic management, authorization and access control, monitoring) involved in accepting and processing thousands of concurrent API calls.
- Essentially the "front door" for applications in your backend. 

---
## Security
AWS 5 main security services 
1. AWS Identity and Access Management (IAM)
2. AWS Certificate Manager (ACM)
3. AWS Shield
4. AWS Key Management Service (KMS)
5. Amazon Cognito

**IAM:**

- Allows you to securely manage access to AWS services and resources.
- You can create users, groups, and permissions that define which actions are allowed and denied for each.

**ACM:**

- Service for creating, manages, and deploying SSL/TLS certificates. 

**Shield:**

- A Distributed Denial of Service (DDoS) protection service 
- Available in two tiers: Standard and Advanced.

**KMS:**

- Create and control the encryption keys 

**Cognito:**

- Provides authentication, authorization, and user management 
- Sign in directly with a user name and password or integrates with Facebook, Google, Microsoft, via SAML

---

## Monitoring
AWS 5 main monitoring services 
1. Amazon CloudWatch
2. AWS X-Ray
3. AWS CloudTrail
4. Amazon Inspector
5. AWS Trusted Advisor

**CloudWatch:**

- Monitoring service for AWS resources 
- Collects and track logs, metrics, and events. 


**X-Ray:**
- Provides tools to view, filter, and gain insights about the requests that your application serves. 
- Helps you understand how your application is performing 
- Shows a map of your application’s underlying components.

**CloudTrail:**

- Helps in compliance, governance, risk auditing, and operational auditing.
- Provides event history of your AWS account activity (includes actions made from AWS Management Console, AWS SDKs, command line tools)


**Inspector:**

- A threat detection service that continuously monitors for malicious activity and unauthorized behavior to protect your AWS accounts and workloads.
- Uses machine learning, anomaly detection, and integrated threat intelligence to identify and prioritize potential threats.

**Trusted Advisor:**

- A resource that can help you reduce cost, increase performance, and improve security by optimizing your AWS environment
- Provides real time guidance to help you provision your resources.

---

**There are many other services provided by AWS across various domains, like IoT, Machine Learning, etc., which are not covered here.**