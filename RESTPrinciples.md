# REST Principles

Representational State Transfer (REST) is an architectural style for designing networked applications. RESTful systems adhere to several principles that guide the design of APIs and interactions between clients and servers. Here are the key REST principles:

1. **Client-Server Architecture**: The system is divided into clients and servers, each with distinct responsibilities. Clients are responsible for the user interface and application logic, while servers are responsible for storing and managing data, application logic, and security.

2. **Statelessness**: Each request from a client to the server must contain all the information necessary to understand and process the request. The server should not maintain any client state between requests. This simplifies server implementation, improves scalability, and enables better caching and load balancing.

3. **Uniform Interface**: RESTful APIs should have a uniform and standardized interface, which simplifies client-server interactions and promotes interoperability. The uniform interface is defined by four constraints:

   - **Resource Identification**: Resources are uniquely identified by URIs (Uniform Resource Identifiers). Each resource should have a stable, unique identifier.

   - **Resource Manipulation through Representations**: Clients interact with resources through representations, such as JSON or XML documents. These representations encapsulate the current state of the resource and may include metadata or hyperlinks.

   - **Self-Descriptive Messages**: Messages exchanged between clients and servers should include metadata (e.g., HTTP headers) that describe the message content, format, and semantics. This enables self-descriptive messages and simplifies message processing.

   - **Hypermedia as the Engine of Application State (HATEOAS)**: Hypermedia controls are embedded within representations and provide links to related resources or actions. Clients navigate the application state by following these hypermedia links, allowing for a dynamic and discoverable API.

4. **Cacheability**: Responses from the server should explicitly indicate whether they are cacheable or not. Caching improves performance and reduces server load by allowing clients and intermediary caches to reuse previously retrieved responses.

5. **Layered System**: The architecture should be composed of multiple layers, where each layer has a specific role and responsibility. Layers can include proxies, gateways, caches, and load balancers. This enables scalability, reliability, and encapsulation of concerns.

6. **Code-On-Demand (optional)**: Servers can optionally provide executable code to clients (e.g., JavaScript), which is executed within the client's runtime environment. This constraint is optional in REST and not commonly used in practice.

By adhering to these principles, RESTful systems can achieve desirable properties such as scalability, reliability, and evolvability. RESTful APIs are widely adopted in web development due to their simplicity, flexibility, and compatibility with existing web standards like HTTP.
