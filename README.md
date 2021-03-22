## Introduction to GraphQL (overview)

#### What is GraphQL?
GraphQL is an open-source data query and manipulation language for APIs, and a runtime for fulfilling queries by using a type system you define for existing data. GraphQL was developed internally by Facebook in 2012 before being publicly released in 2015.

GraphQL provides a complete and understandable description of the data in your API, gives clients the power to ask for exactly what they need and nothing more, makes it easier to evolve APIs over time, and enables powerful developer tools.

#### Difference between GraphQL and Rest.
A REST API is an architectural concept for network-based software. GraphQL, on the other hand, is a query language, a specification, and a set of tools that operates over a single endpoint using HTTP.

With REST, you have to make three requests to different endpoints to fetch the required data. You're also overfetching since the endpoints return additional information that's not needed. In GraphQL on the other hand, you'd simply send a single query to the GraphQL server that includes the concrete data requirements.

#### What is Schema and Resolvers in GraphQL.
* **Schema**
The GraphQL server uses a schema to describe the shape of your data graph. This schema defines a hierarchy of types with fields that are populated from your back-end data stores. The schema also specifies exactly which queries and mutations are available for clients to execute against your data graph.

* **Resolvers**
Resolver is a collection of functions that generate response for a GraphQL query. In simple terms, a resolver acts as a GraphQL query handler. Every resolver function in a GraphQL schema accepts four positional arguments as given below − fieldName:(root, args, context, info) => { result }