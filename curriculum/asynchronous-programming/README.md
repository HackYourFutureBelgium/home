# Asynchronous Programming

[<< Architecture](../architecture/README.md) | [Top](../README.md) | [Web Apps >>](../web-apps/README.md)

> "Synchronous basically means that you can only execute one thing at a time. Asynchronous means that you can execute multiple things at a time and you don't have to finish executing the current thing in order to move on to next one."
>
> - [Mike](https://stackoverflow.com/a/33585047)

---

[examples, exercises and guides](https://github.com/HackYourFutureBelgium/asynchronous-programming)

---

## Learning Objectives

- 🥚 You understand the JavaScript Event Loop, and can demonstrate this by using `setTimeout` and `setInterval` to schedule simple tasks.
- 🥚 You can explain why Asynchronous Programming is important for programs that have _blocking_ and _non-blocking_ tasks.
- 🥚 You can explain the basics of the Client/Server model and HTTP requests and can `fetch` data from RESTful APIs.
- 🥚 You can convert built-in Node modules from consuming callbacks being promises.
- 🐣 You can write and run JavaScript for Node.js or for the Browser. Both environments run JavaScript but they have some important differences!
  - **use cases**: You can explain some use cases that are unique to each runtime.
  - **built-in APIs**: You can list some of the key APIs available in each environment, and why they are not available in the other.
  - **module systems**: You can explain the difference between _CommonJS Modules_ in Node.js and _ES Modules_ in the Browser. You can write and use programs written with either system.
- 🐣 You can trace, refactor and write code that accesses the file system between these 3 different syntaxes:
  1. Callbacks
  2. Promises
  3. `async`/`await`
- 🐣 You can break a problem down into tasks that can be executed in parallel and tasks that must be executed sequentially.
- 🐣 You can write small programs with a Data Access layer that uses data stored in different locations:
  - **Browser**: You can write a small web page that `fetch`es data from a RESTful API and renders it into the DOM.
  - **Node**: You can write a small CLI program that reads user input from `process.argv` and reads/writes the file system.
- 🐥 You can explain the difference between _asynchronous_ anwd _parallel_, and can apply this to reading programs written with JavaScript.
