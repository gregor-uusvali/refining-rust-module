## Domain Driven Design

Domain-driven design (DDD) is a major software design approach, focusing on modeling software to match a domain according to input from that domain's experts. One principle behind DDD is to bridge the gap between domain experts and developers by using the same language to create the same understanding.

## Task

Student has to implementing DDD. This involves the student designing a foldering and code structure for the task that the bracnch focuses on.

Design application architecture:

1. A Domain Layer - The Domain Layer contains the real business logic, but does not contain any infrastructure specific code.
2. An Infrastructure Layer - The Application Layer takes commands from the User Interface Layer and translates these commands to use case invocations on the domain layer.
3. Application Layer - The Infrastructure Layer provides the infrastructure dependent parts for all other layers.
4. Client / User Interface Layer - The Client Layer consumes Application Services and invokes business logic on these services.

Bonus: Model the project with UML.

## References

[Best Practice - An Introduction To Domain-Driven Design](https://learn.microsoft.com/en-us/archive/msdn-magazine/2009/february/best-practice-an-introduction-to-domain-driven-design)

[Domain-driven design](hhttps://en.wikipedia.org/wiki/Domain-driven_design)

[Domain-driven Design Example](https://www.mirkosertic.de/blog/2013/04/domain-driven-design-example/)

## Learning outcomes

After this module the sutudent should have good understanding of design-driven design and implementation of industry standard project layering.
