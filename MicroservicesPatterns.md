# Microservices Patterns

<!-- 
Service Registry & Discovery
API Gateway
Circuit Breaker
Bulkhead
Saga Pattern
Event Sourcing
Choreography vs. Orchestration
Saga Choreography
Polyglot Persistence
Backends for Frontends (BFF)
-->

Microservices architecture offers various patterns to address different concerns such as scalability, resilience, and maintainability. Here are some common microservices patterns:

1. **Service Registry & Discovery**: A central service registry (like Netflix Eureka) where services register themselves, and clients discover services dynamically. This allows for a more flexible and scalable system as services can be added or removed without manual configuration.

2. **API Gateway**: A single entry point for clients to interact with the microservices ecosystem. The API gateway handles client requests, routing them to the appropriate microservices, and often performs tasks like authentication, rate limiting, and protocol translation.

3. **Circuit Breaker**: A pattern to prevent cascading failures in a distributed system. When a service repeatedly fails, the circuit breaker trips and temporarily prevents requests to that service, allowing it to recover. This prevents the entire system from being overwhelmed by continuous failures.

4. **Bulkhead**: Inspired by ship design, this pattern isolates components of an application so that if one fails, it doesn’t bring down the whole system. For microservices, this means partitioning services into different pools of resources, such as thread pools, databases, or networks.

5. **Saga Pattern**: A way to manage transactions that span multiple microservices. Instead of using distributed transactions, which can be complex and have performance implications, the saga pattern breaks down the transaction into a series of smaller, independent steps, each of which is executed by a separate service.

6. **Event Sourcing**: A pattern where the state of a system is determined by a sequence of events. Each service maintains its own database and publishes events to a message broker when its state changes. Other services consume these events to update their own state asynchronously.

7. **Choreography vs. Orchestration**: In choreography, each service publishes events in response to state changes, and other services react to those events independently. In orchestration, a central component (orchestrator) coordinates the interactions between services, determining the order of execution.

8. **Saga Choreography**: Combining the saga pattern with choreography, where each step in the saga is initiated by an event and is responsible for triggering the next step in the saga. This keeps the coordination logic decentralized and avoids the need for a central orchestrator.

9. **Polyglot Persistence**: Recognizing that different microservices may have different data storage requirements, this pattern allows each service to use the most appropriate database technology for its needs, whether that be relational, NoSQL, or something else.

10. **Backends for Frontends (BFF)**: In systems with diverse client requirements (e.g., web, mobile), each type of client may require a different API. BFF pattern involves creating a separate backend service for each type of client, allowing for tailored APIs and better client-server interaction.

These patterns are just a starting point, and real-world microservices architectures often combine multiple patterns to address specific requirements and challenges.
