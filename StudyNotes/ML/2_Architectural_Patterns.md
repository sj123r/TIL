# Architectural Patterns

Created: September 19, 2022 11:32 AM
Tags: ML System Design


[Being a Data Scientist does not make you a Software Engineer!](https://towardsdatascience.com/being-a-data-scientist-does-not-make-you-a-software-engineer-c64081526372)

### Reactive Systems

- Responsive: reacts in a timely manner.
- Resilient: system remains responsive to errors.
- Message Driven: relies on asynchronous message passing.
- Elastic: system stays responsive under varying load.

> IMO: focused more on stability & sustainability
> 

Ex: React

### ****Service Oriented Architecture (SOA)****

Concept: Decomposes business problems into services.

![SOA.png](https://github.com/sj123r/Assets/blob/main/2_Architectural_Patterns/Architectural%20Patterns/SOA.png)

| Component | Description |
| --- | --- |
| Service Provider | publishes a contract that specifies the nature of the service and how to use it. |
| Service Customer | can locate the service metadata in the registry and develop the required client components to bind to it and use it. |
| Orchestrator | a composite service which is responsible for invoking and combining other services |
| Choreography | decentralized approach for service composition, i.e. services interact with the exchange of messages/events. |