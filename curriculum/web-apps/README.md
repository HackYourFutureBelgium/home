# 11. Web Apps

[<< Asynchronous Programming](../asynchronous-programming/README.md) | [Top](../README.md) | [Databases >>](../databases/README.md)

> ![client/server model](./assets/client-server-model.svg)
>
> - [wikipedia](https://en.wikipedia.org/wiki/Client%E2%80%93server_model#/media/File:Client-server-model.svg)

---

[examples, exercises and guides](https://github.com/HackYourFutureBelgium/web-apps)

---

## Learning Objectives

- 🥚 **HTTP**: You can explain these basic notions of the HTTP protocol, the main verbs, headers, ...
- 🥚 **Client/Server Architecture**: You can draw a diagram of your project explaining how the front- and back-ends connect, and can generalize this idea to any web app they use.
- 🥚 **Persistence**: You can explain what persistence is and how it is used in the backend of a web app. You can implement persistence using the backend's file system.
- 🥚 **Postman**: You can use Postman to test and inspect HTTP request/response cycles.
- 🥚 **VSCode Debugger**: You can use breakpoints to pause and step through a Node.js scripts and APIs using the VSCode debugger.
- 🥚 **Promisification**: You can convert built-in node modules from consuming callbacks being `async` functions.
- 🥚 **NPM Modules**: You can find, install, require and use an NPM module in your projects
- 🥚 **Function Roles**: You can explain and apply these 4 function roles in your backend code:
  - _controllers_: like event handlers, but for HTTP requests. (like event handlers in the frontend)
  - _middleware_: do things with a request before it is handled. (no frontend analogy)
  - _data access_: read/write from your data source and return the prepared data, in this module the data source is the file system. (like api calls in the frontend)
  - _logic_: pure functions that transform data and have unit tests. (same as for the frontend)
  - _utils_: functions with side-effects that do one helpful thing. (like procedures in the frontend)
- 🥚 **Express.js**: You can ...
  - listen a new server
  - use middleware
  - `.get`, `.post`, `.put`, `.delete`
  - route params
  - request body
  - send response
  - Express Router
  - static serving
- 🥚 **Entry Points**: You can identify the entry points for your app:
  - _Initialization_: npm scripts, first file, configuration points, server listening
  - _Request/Response Cycle_: first middleware, logging, routes, error handling
- 🥚 **API Documentation**: You can use JSDoc-style comments to document your API, and a documentation script to build API documentation
- 🐣 **File System**: You can read, write and append to .txt files. You can can parse, manipulate and re-save data stored in a .json file using the built-in `fs` and `util.promisify` functions.
- 🐣 **Data Validation**: You can validate data sent in a request to the backend before saving it to a .json file
- 🐣 **RESTful Routes**: You can implement RESTful routes in Express.js, including using the correct `app._` verbs.
- 🐣 **Authentication**: You can explain the principles of authentication and can contribute to a group project that has basic authentication
- 🐣 **Authentication vs. Authorization**: You can explain the difference and how it is implemented in your projects
- 🐣 **Environmental Variables**: You can explain what an environmental variable is, what they're used for, and how they're configured
- 🐣 **Backend Configuration**: You can use environmental variables to launch your backend in different modes
- 🐥 **Asynchronous Callbacks**: You can read, trace and complete simple scripts that use callbacks to work with the file system
- 🐥 **CI Deployment**: You can set up a deployment for your web apps and connect it to your repository using a CI action so `main`/`master` is always deployed.
- 🐔 **CLI Apps**: You can complete a simple CLI app that takes user input from the command line and accesses the file system
- 🐔 **`node-fetch`**: You make API requests from the backend, and use the data in your web apps
- 🐔 **Testing Routes**: You can explain how tests for API routes work, and can write routes that pass given tests. You can also write tests for a route that already exists.
