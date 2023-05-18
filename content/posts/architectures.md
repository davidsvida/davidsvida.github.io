---
title: "Architectures"
date: 2023-04-30
description: "Exploring Software Architectures"
weight: 3
showToc: false
TocOpen: false
draft: false
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

I like to group architectures into 2 groups: Coupled architectures and Decoupled architectures. 

A decoupled architecture is one in which an applications components are weakly associated with each other. Coupled would be the opposite. 

---
### Coupled architectures
-   Monolithic architecture (tightly coupled)
-   Serverless architecture (loosely coupled)

### Decoupled architectures

-   [Microservices architecture](https://davidinsider.com/posts/microservices/)
-   Event-driven architecture
-   Service-oriented architecture

---
### Definitions 

**Monolithic architecture** is a *tightly* coupled architecture where all the components of an application are deployed as a single unit. 

**Serverless architecture** is a *loosely* coupled architecture where the application is built using functions that are executed in a serverless environment.

**Microservices architecture** is a decoupled architecture where the application is composed of *independent* services that communicate with each other through APIs. 

**Event-driven architecture** is a decoupled architecture where services communicate with each other *asynchronously* through events. 

**Service-oriented architecture** is a decoupled architecture where services are designed to be reusable and accessed over a network. 

---


### Which one should I choose ? 

-   Monolithic architecture: when the application is simple and does not require the flexibility and scalability of microservices.

-   Serverless architecture: when the application has highly variable workloads or unpredictable usage patterns, and *cost-effectiveness* is a priority.

-   Microservices architecture: when the application is complex and requires the flexibility and scalability of independent services, and the team is experienced in building distributed systems.

-   Event-driven architecture: when the application requires real-time event processing and needs to scale quickly in *response* to changing demand.

-   Service-oriented architecture: when the application needs to *integrate* with multiple systems and services, and reusability and accessibility of services are important.


---

### You can also mix... 

Common hybrid architectures include 

-   microservices and serverless
-   microservices and event-driven
-   microservices and service-oriented
-   monolithic and microservices
---




