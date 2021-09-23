# 9. Architecture

[&lt;&lt; Separation of Concerns](separation-of-concerns/) \| [Top](./) \| [Asynchronous Programming &gt;&gt;](asynchronous-programming.md)

> "We're talking about boxes and lines. We're talking about the big picture."
>
> * [GetCloudSkills](https://www.youtube.com/watch?v=i7aKW7YNOxY)

[examples, exercises and guides](https://github.com/HackYourFutureBelgium/architecture)

## Learning Objectives

* 🥚 **State**: You understand the concept of state as the data stored in your application _at each moment_. You can explain how state is _rendered_ into a user interface, and can explain how each user interaction reads/writes from state.
* 🥚 **Persistence**: You can explain what _persistence_ means and how it can be implemented in the browser using `localStorage`. When you encounter a bug in your code based persisted data, you can use `localStorage.clear()` and a page refresh to reset your project's state.
* 🥚 **Data-First Development**: You understand applications as data + user interactions. You can demonstrate this by _starting_ your planning process with the data you will need and building a user interface to show that data to a user.
* 🥚 **Architecture & Layers**: You can explain what software architecture is and the importance of layers for testing, collaboration, and maintenance. These are the layers you will learn to use, from the "back" to the "front":
  * _**Data Access**_: This layer is responsible for _persisting_ your data, reading and writing from wherever it is stored. This layer has no fancy logic, it just gets things and puts things away again.
  * _**Business Logic**_: This layer is responsible for all the important _actions_ in your application. The Business Logic layer _does not ever_ interact directly with the user or the user interface. Instead it takes in JS data from the Presentation layer, reads/writes state via the Data Access layer, and returns new data for the Presentation Layer to render.
  * _**Presentation**_: This is the layer you studied in Separation of Concerns. It renders program state for the user, and handles their interactions. It's possible to different presentation layers for the same business logic!
* 🥚 **Abstraction**: You can explain what _abstraction_ is and demonstrate it in the source code for this module's projects.
* 🥚 **Function Roles**: You can use these new function roles while planning and developing your projects:
  * _**Data Access**_: Functions that insert \(create\), find \(read\), save \(update\), remove \(delete\) entries in your saved data. These are provided for you in this module. Data Access functions can only import `utils` and other data access functions.
  * _**Business Logic**_: Functions that take in JS data, read/update state, and return new data. these can be called from handlers, components, or other business logic. Business Logic functions can only import `utils`, `data-access` and other `business-logic` functions.
  * _**Handlers**_: The same role as in Separation of Concerns, only now with a few more restrictions. Handlers _can not_ use _data_ directly or use _data access_ functions. They can only import _Business Logic_, _Components_ and _Utils_.
  * _**Custom Events**_: Functions that return a `new CustomEvent` with your choice of `.type`, and data stored in the it's `.details` property. These will be very helpful for creating testable and reuseable components in your frontend. Custom Events can only import `utils`
* 🥚 **Development Strategies**: You can write development strategies with each user story broken into _business logic_, _interface_ and _interaction_ tasks.
* 🥚 **Development Steps**: In this module you will learn to build your projects backwards from the "inside" out:
  1. Plan and write your data \(_.json_ file and schema\)
  2. Plan, write and test your business logic
  3. Plan and write a static user interface \(HTML+CSS\)
  4. Develop interactions for the interface \(listeners, handlers, components, custom events\)
* 🥚 **Other People's Code**: You will learn to use code other people wrote by reading their documentation and understanding their source code. This will happen when you use the Data Access layer provided by HYF, and when you use the functions written by your group members.
* 🐣 **Nested Data**: Given a nested data structure containing arrays, objects and primitive values, you can 1\) access a given value 2\) update a given entry 3\) filter the data
* 🐣 **Matching a JSON Schemas**: You can write an object or array that matches a JSON schema.
* 🐣 **Using a Library**: You can select which functions from the `/data-access` library to use in your Business Logic functions. This includes reading the documentation, tests and source code to understand how the Data Access functions work.
* 🐣 **Stateful Testing**: You can pass and write unit tests for stateful functions - using `beforeEach` to reset state before each test, and testing for the _correct_ side-effects in state.
* 🐥 **TDD + Reverse Engineering**: Given unit tests for the _business logic_ and an obfuscated demo of the interface, you can build a working application that passes the tests and matches the demo.
* 🐥 **Writing a JSON Schemas**: You can write a JSON schema that matches several data instances.

