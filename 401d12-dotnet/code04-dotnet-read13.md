# Code 401 ASP.NET
## Reading 13
##### (All My Notes are attributed/sourced from the Resources directly preceding them.)

<br>
<br>
<br>

### Summary
* Dependency (Objects depending on other objects) have problems such as if something needs to change then you would have to change the Classes that the Object is dependent upon and possibly multiple other connected classes.
* Dependency Injection addresses these problems via several methods
  * interface or abstract base class
  * registration of a service container
  * framework takes responsibility for creating the instances
* A well designed Repository setup makes it easier to find and test pieces of the application being developed.
* Repository Patterns have two purposes
  * Abstraction of the data layer
  * Centralising the handling of the domain objects
* SOLID Coding stands for:
  * Single Responsibility Principle - every method/class in your app should have one single job.
  * Open/Close Principle - method/class should be open for extention, but closed to modification
  * Liskov Substitution Principle - objects in your app should be replaceable by any type derived from it without breaking the app.
  * Interface Segregation Principle - do not force any reliance on interfaces that are not used.
  * Dependency Inversion Principle - code should depend on abstractions not concrete implementation
* SOLID is important because it creates code that is easily testable.

<br>
<br>

### Resources
* #### __Dependency injection in ASP.NET Core__
  * ##### Author:  Microsoft Docs
  * ##### [Article Source](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/dependency-injection?view=aspnetcore-5.0)

* #### __Design the infrastructure persistence layer__
  * ##### Author:  Microsoft Docs
  * ##### [Article Source](https://docs.microsoft.com/en-us/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/infrastructure-persistence-layer-design#the-repository-pattern)

* #### __Repository Design Pattern__
  * ##### Author:  Erik Bergman
  * ##### [Article Source](https://medium.com/@pererikbergman/repository-design-pattern-e28c0f3e4a30)

* #### __30 Days of TDD: Day Five – Make Your Code SOLID__
  * ##### Author:  James Bender
  * ##### [Article Source](https://www.telerik.com/blogs/30-days-of-tdd-day-five-make-your-code-solid)

* #### __Why SOLID Matters__
  * ##### Author:  Phil Japikse
  * ##### [Article Source](https://www.telerik.com/blogs/why-solid-matters)

* #### __The S.O.L.I.D Principles in Pictures__
  * ##### Author:  Ugonna Thelma
  * ##### [Article Source](https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898)

<br>
<br>
<br>

[<-- Back](../README.md)
