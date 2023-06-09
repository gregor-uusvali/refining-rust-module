# Microservices - a guide book

Microservices - getting to know them

Microservices - also known as the microservice architecture - is an architectural style that structures an application as a collection of services that are:
Independently deployable
* Loosely coupled
* Organised around business capabilities
* Owned by a small team
* The microservice architecture enables an organisation to deliver large, complex applications rapidly, frequently, reliably and sustainably - a necessity for competing and winning in today’s world. 

As defined by Amazon: “Microservices are an architectural and organisational approach to software development where software is composed of small independent services that communicate over well-defined APIs. These services are owned by small, self-contained teams.”

Monolith - what is it

A centralised application. An architecture that structures the application as a single deployable/executable component that uses a single database. The component contains all of the application’s subdomains. Since there’s a single component, all operations are local.

The Pros and Cons

The Pros:
* A MS is scalable, agile and more efficient in use for big teams.
* Can be structured into small, autonomous teams. 
* Fault isolation -  if an individual microservice becomes unavailable, it won't disrupt the entire application, as long as any upstream microservices are designed to handle faults correctly.
* Data isolation. It is much easier to perform schema updates, because only a single microservice is affected. In a monolithic application, schema updates can become very challenging, because different parts of the application might all touch the same data, making any alterations to the schema risky.
* Scalability. Services can be scaled independently, letting you scale out subsystems that require more resources, without scaling out the entire application. Using an orchestrator such as Kubernetes or Service Fabric, you can pack a higher density of services onto a single host, which allows for more efficient utilisation of resources.

The Cons:

* The complexity and testing of a MS architecture is what draws it apart from Monoliths. There needs to be a deeper understanding of the different systems used and compatibility.  Existing tools are not always designed to work with service dependencies. Refactoring across service boundaries can be difficult. It is also challenging to test service dependencies, especially when the application is evolving quickly.
* Management. To be successful with microservices requires a mature DevOps culture. Correlated logging across services can be challenging. Typically, logging must correlate multiple service calls for a single user operation.
* Versioning. Updates to a service must not break services that depend on it. Multiple services could be updated at any given time, so without careful design, you might have problems with backward or forward compatibility.
* Skill set. Microservices are highly distributed systems. Carefully evaluate whether the team has the skills and experience to be successful.

Sources:
https://microservices.io/
https://aws.amazon.com/microservices/ 
https://learn.microsoft.com/en-us/azure/architecture/guide/architecture-styles/microservices 
