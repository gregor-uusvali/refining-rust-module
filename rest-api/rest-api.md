# RESTful API

## Definition of a RESTful API
- An API, Application Programming Interface, is a set of defined rules that enable different applications to communicate with each other. In simpler terms, think of an endpoint/url that one service call and another service is running to response behind that endpoint/url
- An API will be qualified to be called RESTful, or just REST, as long as it meets the following 6 principle/criterias. These requirements are format and language agnostic, making the implementation very versataile:
  1. Uniform interface. All API requests for the same resource should look the same, no matter where the request comes from. The REST API should ensure that the same piece of data, such as the name or email address of a user, belongs to only one uniform resource identifier (URI). Resources shouldn’t be too large but should contain every piece of information that the client might need.
  2. Client-server decoupling. In REST API design, client and server applications must be completely independent of each other. The only information the client application should know is the URI of the requested resource; it can't interact with the server application in any other ways. Similarly, a server application shouldn't modify the client application other than passing it to the requested data via HTTP.
  3. Statelessness. REST APIs are stateless, meaning that each request needs to include all the information necessary for processing it. In other words, REST APIs do not require any server-side sessions. Server applications aren’t allowed to store any data related to a client request.
  4. Cacheability. When possible, resources should be cacheable on the client or server side. Server responses also need to contain information about whether caching is allowed for the delivered resource. The goal is to improve performance on the client side, while increasing scalability on the server side.
  5. Layered system architecture. In REST APIs, the calls and responses go through different layers. As a rule of thumb, don’t assume that the client and server applications connect directly to each other. There may be a number of different intermediaries in the communication loop. REST APIs need to be designed so that neither the client nor the server can tell whether it communicates with the end application or an intermediary.
  6. Code on demand (optional). REST APIs usually send static resources, but in certain cases, responses can also contain executable code (such as Java applets). In these cases, the code should only run on-demand.

## Best practices
- HTTP methods and its relation with REST
  - In HTTP there are five methods that are commonly used in a REST-based Architecture i.e., `POST`, `GET`, `PUT`, `PATCH`, and `DELETE`. These correspond to create, read, update, and delete (or CRUD) operations respectively.
- An **idempotent** HTTP method is a HTTP method that can be called many times without different outcomes. It would not matter if the method is called only once, or ten times over. A `PUT` request should should always be idempotent.
- [DOs and DONTs with real endpoint example](https://medium.com/creative-black-pug-studio/restful-apis-5b0944900e6a)


## REST API with Java
### Common framework
[Spring Boot](https://spring.io/projects/spring-boot) is a framework in java that helps you to bring up a project quickly, it's not REST-specific, but commonly used to build RESTful web service due to the convinience and extendability that it provides
### Practicle example
[Building a RESTful Web Service with SpringBoot](https://spring.io/guides/gs/rest-service/)


## REST API with Python
### Common framework
[Django](https://www.djangoproject.com/)
### Practicle example

## REST API with Go
### Common framework
[Gin](https://github.com/gin-gonic/gin#gin-web-framework)
### Practicle example

## Reference
- [IBM: What's an API](https://www.ibm.com/topics/api)
- [IBM: What's a RESTful API](https://www.ibm.com/topics/rest-apis)
- [Amazon: What's a RESTful API](https://aws.amazon.com/what-is/restful-api/)
- [Redhat: What's a RESTful API](https://www.redhat.com/en/topics/api/what-is-a-rest-api)
- [Geek for Geek](https://www.geeksforgeeks.org/rest-api-introduction/)