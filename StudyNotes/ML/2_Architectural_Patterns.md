# Architectural Patterns

Created: September 19, 2022 11:32 AM
Tags: ML System Design

Reference: [Being a Data Scientist does not make you a Software Engineer!](https://towardsdatascience.com/being-a-data-scientist-does-not-make-you-a-software-engineer-c64081526372)

### **Reactive Systems**

- Responsive: reacts in a timely manner.
- Resilient: system remains responsive to errors.
- Message Driven: relies on asynchronous message passing.
- Elastic: system stays responsive under varying load.

> IMO: focused more on stability & sustainability
> 

Ex: React

### **Service Oriented Architecture (SOA)**

Concept: Decomposes business problems into services.

![SOA.png](https://github.com/sj123r/Assets/blob/main/2_Architectural_Patterns/Architectural%20Patterns/SOA.png)

| Component | Description |
| --- | --- |
| Service Provider | publishes a contract that specifies the nature of the service and how to use it. |
| Service Customer | can locate the service metadata in the registry and develop the required client components to bind to it and use it. |
| Orchestrator | a composite service which is responsible for invoking and combining other services |
| Choreography | decentralized approach for service composition, i.e. services interact with the exchange of messages/events. |

### **Lambda Architecture**

![Lambda_Architecture.png](https://github.com/sj123r/Assets/blob/main/Lambda_Architecture.png)

Lambda Architecture uses real-time and historically aggregated batched data in order to include data generated in the last second. This means data generated in the last second, minute, hour can be processed in that analysis by only accepting incoming data(not all data).

### **Microservice Architecture**

![Microservice.png](https://github.com/sj123r/Assets/blob/main/Microservice.png)

Microservice Architecture is an architectural style that structures an application as a collection of small, autonomous, loosely coupled and collaborating services, modelled around a business domain.

### **Representational State Transfer (REST) Architecture**

![Rest.png](https://github.com/sj123r/Assets/blob/main/Rest.png)

REST is an architectural style for developing web services and it builds upon existing features of the internet’s HTTP. It allows transferring, accessing and manipulating textual data representations, in a stateless manner i.e. applications can communicate agnostically.