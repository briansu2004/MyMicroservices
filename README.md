# MyMicroservices

- [My Microservices Projects](#my-microservices-projects)
  - [Project 10](#project-10)
  - [Project 9](#project-9)
- [Microservices Patterns](#microservices-patterns)
- [Microservices Principles](#microservices-principles)
- [Microservices Testing Strategies](#microservices-testing-strategies)
- [Microservices Data Management Strategies](#microservices-data-management-strategies)
- [REST Principles](#rest-principles)
- [Domain Modelling](#domain-modelling)
- [Distributed Application Runtime (Dapr)](#distributed-application-runtime-dapr)
- [OData standard](#odata-standard)
- [Polyglot](#polyglot)
- [Microsoft Entra ID](#microsoft-entra-id)

## My Microservices Projects

### Project 10

REST API, API Gateway

### Project 9

GraphQL

## [Microservices Patterns](MicroservicesPatterns.md)

## [Microservices Principles](MicroservicesPrinciples.md)

## [Microservices Testing Strategies](MicroservicesTestingStrategies.md)

## [Microservices Data Management Strategies](MicroservicesDataManagementStrategies.md)

## [REST Principles](RESTPrinciples.md)

## Domain Modelling

Domain modeling is the process of creating a conceptual representation of a problem domain within a specific context or organization. It involves identifying and defining the key entities, attributes, relationships, and behaviors that are relevant to the problem being solved. Domain modeling is a crucial step in software development, especially in domains where the problem is complex or poorly understood.

Here's a step-by-step guide to domain modeling:

1. **Identify the Domain**: Determine the scope and boundaries of the problem domain. Understand the business context, stakeholders, and goals.

2. **Gather Requirements**: Collect requirements from stakeholders, including business users, domain experts, and technical teams. Document use cases, scenarios, and user stories to capture the functional and non-functional requirements.

3. **Identify Entities**: Identify the main entities or objects within the domain. These could be tangible things like customers, products, orders, or intangible concepts like policies, transactions, or events.

4. **Define Attributes**: For each entity, define the relevant attributes or properties that describe its characteristics. Consider both intrinsic attributes (e.g., name, description, date) and derived attributes (e.g., total cost, status).

5. **Establish Relationships**: Identify relationships between entities. Relationships describe how entities are connected or interact with each other. Common types of relationships include one-to-one, one-to-many, and many-to-many.

6. **Capture Behavior**: Define the behavior or actions associated with entities. This includes both passive behavior (e.g., data retrieval, calculation) and active behavior (e.g., methods, functions, processes).

7. **Model Constraints**: Identify any constraints or rules that apply to the domain. Constraints could include validation rules, business rules, or integrity constraints that must be enforced by the system.

8. **Refine and Iterate**: Refine the domain model based on feedback from stakeholders and domain experts. Iterate on the model to ensure that it accurately reflects the problem domain and meets the needs of the users.

9. **Validate the Model**: Validate the domain model against the requirements to ensure that it fulfills the functional and non-functional requirements of the system. Identify any inconsistencies or gaps in the model and address them accordingly.

10. **Document the Model**: Document the domain model using appropriate notations and tools. This could include textual descriptions, diagrams (e.g., UML class diagrams), or domain-specific languages.

Domain modeling is an iterative process that often evolves over time as the understanding of the problem domain deepens and new requirements emerge. It serves as a foundation for software design and development, helping to align technical solutions with business needs and ensuring that the resulting software system is both effective and maintainable.

## Distributed Application Runtime (Dapr)

Dapr, or Distributed Application Runtime, is an open-source project designed to make it easier for developers to build microservices-based applications. It provides a set of building blocks for developing applications that are resilient, portable, and scalable across various cloud and edge environments. Dapr abstracts away much of the complexity associated with building distributed systems, offering features like state management, service invocation, pub/sub messaging, and distributed tracing, among others. This allows developers to focus more on writing business logic rather than dealing with the intricacies of distributed systems architecture.

## OData standard

OData (Open Data Protocol) is a standardized protocol for creating and consuming RESTful APIs. It provides a uniform way to expose and access data over the web, enabling interoperability between different systems and platforms. OData builds upon existing web technologies, such as HTTP, JSON, and AtomPub, and defines a set of conventions and best practices for designing APIs.

Here are some key aspects of the OData standard:

1. **RESTful API Design**: OData APIs follow the principles of REST (Representational State Transfer). They use HTTP methods (GET, POST, PUT, PATCH, DELETE) to perform CRUD (Create, Read, Update, Delete) operations on resources, which are identified by URIs (Uniform Resource Identifiers).

2. **Query Options**: OData defines a set of query options that clients can use to customize the shape and content of the data returned by the API. These query options include filtering, sorting, pagination, projections, and expansions (to retrieve related entities).

3. **Metadata**: OData APIs expose metadata that describes the structure of the data, including entity types, properties, relationships, and operations supported by the API. Metadata is typically represented using the OData Common Schema Definition Language (CSDL), which is an XML-based format.

4. **AtomPub and JSON Formats**: OData supports both AtomPub (Atom Publishing Protocol) and JSON (JavaScript Object Notation) formats for representing data. AtomPub is a standardized XML-based format, while JSON is a lightweight and widely used data interchange format.

5. **Entity Data Model (EDM)**: OData defines a data model called the Entity Data Model (EDM), which provides a conceptual framework for describing the structure of data and relationships between entities. The EDM includes entity types, complex types, associations, and navigation properties.

6. **Protocol Extensions**: OData allows for protocol extensions to support additional features or functionality beyond the core specification. These extensions may include custom query options, custom headers, or additional metadata annotations.

7. **Versioning and Compatibility**: OData supports versioning and backward compatibility to ensure that clients and servers can evolve independently over time. Versioning is typically achieved through URI path segments or HTTP headers.

8. **Security**: OData does not define specific security mechanisms but can be used in conjunction with standard security mechanisms such as HTTPS (HTTP Secure), OAuth, or API keys to secure API endpoints and protect sensitive data.

Overall, OData provides a standardized approach to building and consuming RESTful APIs for exposing and accessing data over the web. It simplifies integration between different systems and platforms by providing a common data interchange format and query language.

## Polyglot

"Polyglot" in the context of software development generally refers to using multiple programming languages, frameworks, or technologies within a single project or system. This term can apply to various aspects of software development, including:

1. **Polyglot Programming**: Developers write different parts of an application using different programming languages. For example, using Python for the backend, JavaScript for the frontend, and SQL for database queries.

2. **Polyglot Persistence**: As mentioned earlier, polyglot persistence involves using multiple types of data storage technologies (relational databases, NoSQL databases, key-value stores, etc.) within a single application or system. Each data storage technology is chosen based on its suitability for specific data storage requirements.

3. **Polyglot Microservices**: In microservices architecture, different microservices within the same system may be implemented using different programming languages or frameworks. This approach allows teams to select the most appropriate technology for each microservice based on its requirements and constraints.

4. **Polyglot Integration**: Applications often need to integrate with various external systems and APIs, which may use different technologies and protocols. Polyglot integration involves using different integration techniques and technologies (such as REST, SOAP, GraphQL, messaging queues) to interact with these external systems.

Polyglot approaches offer flexibility, allowing developers to leverage the strengths of different technologies and tools to solve specific problems within a project. However, they can also introduce complexity in terms of development, deployment, and maintenance. Therefore, it's essential to carefully consider the trade-offs and potential challenges associated with polyglot development before adopting it in a project.

## Microsoft Entra ID

Microsoft Entra ID (formerly known as Microsoft Azure Active Directory or Azure AD) is a cloud-based identity and access management (IAM) solution. It is a directory and identity management service that operates in the cloud and offers authentication and authorization services to various Microsoft services such as Microsoft 365, Dynamics 365, and Microsoft Azure.[1] Entra ID provides users with single sign-on experience, regardless of whether their applications are cloud-based or on-premises.
