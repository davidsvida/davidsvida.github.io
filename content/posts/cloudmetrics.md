---
title: "Cloud Metrics"
date: 2023-06-09
showToc: false
TocOpen: false
draft: false
searchHidden: false
hidemeta: false
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

Metrics are measures of quantitative assessment commonly used for comparing, and tracking performance or production. 

In cloud computing, we use cloud monitoring to track these cloud metrics. Monitoring is a broad term that refers to the process of collecting/analyzing data.


---

## Cloud Monitoring

Cloud monitoring is basically tracking cloud elements (applications, networks, services, infrastructure) in an attempt to ensure their availability, performance, and security.  


Let's look break cloud monitoring down into sections. 

#### 1. Performance Metrics:

Tracks the speed and functionality

- Latency: This measures the response-time. 
- Throughput: Processing a system can perform in a given amount of time. 
- Error rates: Frequency of errors in the system. 


#### 2. Utilization Metrics:

Tracks resource usage

- CPU Utilization: How much CPU capacity is being used
- Memory Utilization: How much system memory is being used.
- Disk Utilization: How much disk space is being used.
- Network Utilization: How much network bandwidth is being used. 

#### 3. Availability Metrics: 

Tracks system uptime and downtime

- Uptime: The amount of time a system is operational.
- Downtime: The amount of time a system is not operational.


#### 4. Cost Metrics:

Tracks the financial aspects 

- Cost per service: See the cost for individual cloud service.
- Cost per resource: See the cost of individual resources (instances, storage, data transfer)
- Cost efficiency: Assesses the cost-effectiveness of both services and resources.

---


## Monitoring Services
- AWS provides CloudWatch
- Azure offers Azure Monitor
-  Google Cloud has Google Cloud Monitoring


<h3 style="text-align: center">Besides collecting metrics, you should do something with those metrics: set up dashboards/reports, notifications/alerts</h3>

