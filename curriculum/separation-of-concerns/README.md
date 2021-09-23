# 8. Separation of Concerns

[&lt;&lt; Behavior, Strategy, Implementation](../behavior-strategy-implementation/) \| [Top](../) \| [Architecture &gt;&gt;](../architecture.md)

> "The most important principle in Software Engineering is the Separation of Concerns \(SoC\): The idea that a software system must be decomposed into parts that overlap in functionality as little as possible."
>
> * [Effective Software Design](https://effectivesoftwaredesign.com/2012/02/05/separation-of-concerns/)

[examples, exercises and guides](https://github.com/HackYourFutureBelgium/separation-of-concerns)

## Learning Objectives

* 🥚 **event-driven programming**: identify the concept in a JS program via listeners & handlers
* 🥚 **entry points**: describe what an entry point is, there are 2 kinds in the programs for this module - initialization & interaction. identify them in a program
* 🥚 **function roles**: describe what function roles are and why they're important. they can identify a function's role given checklists for each role covered in this module:
  * _listeners_: functions that attach event listeners to the DOM
  * _handlers_: entry point for user interactions
  * _utils \(utilities\)_: pure functions to help do things with data
  * _components_: render data into DOM elements to display for the user
* 🥚 **DOM access**: You read and write values from the DOM in an event handler
* 🥚 **es5 vs. es6**: You can demonstrate the change in developer-experience pre and post es6 by stepping through in the debugger and explaining differences in scoping \(global vs. script, block vs. local, modules\) between two programs with identical user experience but different implementations.
* 🥚 **Scope Hierarchy**: You is comfortable navigating different scopes in the browser's debugger to understand an existing application \(script, module, closure, local, block\)
* 🥚 **Code Splitting**: You can ES Modules to split your code into multiple files & folders according to function role, data, listeners and initialization. They can use generated dependency diagrams and documentation to understand and navigate this folder structure.
* 🥚 **Dependency Graphs**: You can use a project's dependency graph to understand how it is organized and to navigate the source code.
* 🥚 **Development Strategies**: You can write development strategies that have all of the program's data defined at the beginning, and separate each user story into _interface_ and _interaction_ tasks.
* 🐣 **Naming Functions**: You can come up with clear and helpful names for the functions in your program. A good function name will take into account the function's role and the program's domain
* 🐣 **DOM manipulation**: You can manipulate the DOM when implementing level-appropriate user interactions
* 🐣 **Isolating Components**: You can use a `test.html` file to render your components with different inputs
* 🐣 **Forms**: You can do basic handling of form data via `event.target.form`
* 🐣 **Handling events**: You can use the `event` argument to process user interactions, including bubbled events using `event.target`
* 🐣 **Passing Component Unit Tests**: You can write vanilla DOM component functions to pass provided unit tests
* 🐣 **refactoring**: refactor a single-script tutorial-style web page into multiple files using imports and exports
* 🐥 **reverse-engineering**: You can incrementally reverse-engineer a level-appropriate user interaction following these steps: ui -&gt; listener -&gt; handler \(-&gt; logic and/or -&gt; component\)
* 🐔 **From Spec**: given user stories, You can develop a site from scratch using a template repository.
* 🐔 **Writing Component Unit Tests**: You can write unit tests to validate your component functions using BDD syntax

![draino in the fridge](../../.gitbook/assets/draino-in-the-fridge.png)

