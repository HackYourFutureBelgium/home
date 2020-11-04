# Java


## Learning Goals

The students can:

- Create a console based functional application;
- Manage external dependencies using Maven;
- Use Unit Testing to verify system behavior;
- Create a professional web application using Spring Boot;

> Open topics
> - What else should we add to the Masterclass?
> - Order of the topics. Might want to move up testing before dependency management or even all the way to the front (learning by writing unit tests)

## Topics

### Base Java and Object Oriented Programming

Introduction of the base concepts in Java

- What is the JVM?
- How is Java different from JavaScript? (Assuming previous experience of some students)?
- What IDEs exist? (Teaching Note: I see a great opportunity here to first use JShell, then move on)
- Code structures (If/else, for, etc.)
- Object oriented Programming


> Open topics:
> - What IDE to use? (IntelliJ / VSCode / Eclipse)
> - How do we differentiate between starters and alumni of the Javascript/Node Bootcamp?

 ### Dependency management

 Just like there is NPM for Javascript, there a better ways to handle dependencies than to just "copy-paste" dependencies into your project.

 - How are applications packaged in Java?
 - Where to find dependencies?
 - How can we Automatically download and include dependencies with Maven?
 - How to use Maven to create your own packages?


 > Open topics:
 > - How deep do we want to get into building with Maven? 
 > - Maven VS Gradle

 ### Testing

Making sure your code works before we ship it is important. In this module we'll discuss

- Testing Pyramid
- Why do unit testing? 
- Writing tests with JUnit
- The 3 A's (Arrange/Act/Assert)
- Handling difficult to test code with Mockito (Mocks and stubs)


> Open topics:
> - Is TDD going too far?
 

### Spring Boot

- What is Spring?
- What is Spring Boot?
- What is Dependency Injection / IoC?
- How do we create a REST API?
- How do we connect to other APIs?
- How can we connect to a database?
- Testing in Spring

> Open topics:
> - I'm not to sure about the scoping here since Spring can be quite a lot to learn (Data/Cloud/Monitoring/etc.). Even connecting to a SQL database implies knowledge of JPA (which is not handled before).

## Resources

- Introduction Java Course by Angie Jones: https://testautomationu.applitools.com/java-programming-course
- Spring Boot (slides for lessons in a classroom, should still update these) by Tom Cools: https://tomcools.be/pdf/AP-Spring-Session.pdf
