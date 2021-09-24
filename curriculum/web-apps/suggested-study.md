# Suggested Study

Helpful resources for this module

> Are we missing a great set of exercises? Send a PR!

## HTTP Statuses

- [In 60 Seconds](https://www.youtube.com/watch?v=GrNrcmD6HLA)
- [httpstatuses.com](https://httpstatuses.com/)
- [wikipedia](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes)
- [http.cat](https://http.cat/)

## NPM

- [What is it? How to use it?](https://www.youtube.com/watch?v=8Rmj5UY5mJk)
- packages for fun:
  - [cowsay](https://github.com/piuccio/cowsay) - make cows say things
- packages for serious:
  - [node-fetch](https://github.com/node-fetch/node-fetch) - Make API requests from Node
  - [express](https://github.com/expressjs/express) - Minimalist web framework for node
  - [body-parser](https://github.com/expressjs/body-parser) - Parse HTTP request body into JS object
  - [cors](https://github.com/expressjs/cors) - Cross Origin Resource Sharing for Express
  - [morgan](https://github.com/expressjs/morgan) - logging for Express
  - [joi](https://github.com/hapijs/joi), [tv4](https://github.com/geraintluff/tv4) - JSON schemas & validation

## Debugging Node in VSCode

> [Postman](https://www.postman.com/) - use your APIs without a frontend

- [Getting started with Node.js debugging in VS Code](https://www.youtube.com/watch?v=2oFKNL7vYV8)
- [Burke Holland](https://www.youtube.com/watch?v=NW2HG9C_mZc)
- [VSCode Channel Intro](https://www.youtube.com/watch?v=2oFKNL7vYV8)
- [James Q Quick](https://www.youtube.com/watch?v=yFtU6_UaOtA)
- [CodeSpace, 2 Ways](https://www.youtube.com/watch?v=N8O-Yf3hc-A)

## Node.js

- **101**
  - [Mosh: Node.js in 1 hour](https://www.youtube.com/watch?v=uVwtVBpw7RQ&list=PLTjRvDozrdlydy3uUBWZlLUTNpJSGGCEm&index=1)
  - [Traversy: Node for Absolute Beginners](https://www.youtube.com/watch?v=U8XF6AFGqlc)
  - [Traversy: Node.js Crash Course](https://www.youtube.com/watch?v=fBNz5xF-Kx4)
  - [NetNinja: Node Js Crash Course](https://www.youtube.com/playlist?list=PL4cUxeGkcC9jsz4LDYc6kv3ymONOKxwBU)
  - [`argsv`](https://nodejs.org/en/knowledge/command-line/how-to-parse-command-line-arguments/) - Use command line arguments in Node
- **Built-In Modules**
  - [The file system](https://vimeo.com/414475261) (first 20 minutes)
  - references
    - [assert](https://nodejs.org/api/assert.html) - Test values in Node.js
    - [fs](https://nodejs.org/api/fs.html) - Read & write form the file system
    - [path](https://nodejs.org/api/path.html) - Manipulate file paths
    - [util.promisify](https://nodejs.org/api/util.html#util_util_promisify_original) - Convert functions that take callbacks into Promises
- **API Calls**
  - [node-fetch](https://www.npmjs.com/package/node-fetch): a module for using `fetch` syntax in Node.js
  - To study a full app with `node-fetch`, head over to [weather-it-promised](../integrate/weather-it-promised) & [weather-it-async-await](../integrate/weather-it-async-await)
  - [/node-fetchemon](./node-fetchemon) (exercises to practice `node-fetch`)

## About Servers

- Middleware: [tutorialspoint](https://www.tutorialspoint.com/expressjs/expressjs_middleware.htm), [express.js guide](https://expressjs.com/en/guide/using-middleware.html), [writing middleware (video)](https://www.youtube.com/watch?v=msw1D8oSw5M)
- Static Serving: [alligator article](https://alligator.io/nodejs/serving-static-files-in-express/), [codedamn video](https://www.youtube.com/watch?v=7UErZ43jzrU)
- Error Handling Middleware:
  - [Handling Errors in Express](https://zellwk.com/blog/express-errors/)
  - [REST API Tutorial (Node, Express & Mongo) #10 - Error Handling](https://www.youtube.com/watch?v=w1V2SdzdQBs)
- CORS: [Cross Origin Resource Sharing](https://www.youtube.com/watch?v=x_Z6iYY5ibc)
- HTTP Statuses
  - [httpstatusdocs](https://httpstatusdogs.com/)
  - [HTTP Request Status Code Guide](https://www.youtube.com/watch?v=VLH3FMQ5BIQ)
  - [In 60 Seconds](https://www.youtube.com/watch?v=GrNrcmD6HLA)
  - [httpstatuses.com](https://httpstatuses.com/)
  - [wikipedia](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes)
  - [http.cat](https://http.cat/)

## Express

- [What is Express?](https://www.besanttechnologies.com/what-is-expressjs)
- [LearnWebCode](https://www.youtube.com/watch?v=z7ikpQCWbtQ)
- [Traversy: Express.js Crash Course](https://www.youtube.com/watch?v=L72fhGm1tfE)
  [Build RESTful APIs with Node and Express](https://www.youtube.com/watch?v=pKd0Rpw7O48) by Mosh
- How To Build a Job Search App (Node, APIs, Vanilla JS): [video](https://www.youtube.com/watch?v=v7cprTuAnlA), [code](https://github.com/codebubb/job-search-app/)
- Error Handling
  - [The Net Ninja](https://www.youtube.com/watch?v=w1V2SdzdQBs)
  - [Andrew Mead](https://www.youtube.com/watch?v=R4uiu3fR38I)
  - [Devnami](https://www.youtube.com/watch?v=pYj48mDXHBU)
- `Router`
  - [Scotch.io](https://scotch.io/tutorials/learn-to-use-the-new-router-in-expressjs-4)
  - [Hungry Turtle](https://www.youtube.com/watch?v=paNikhYqdz0)
  - [Rithm School](https://www.youtube.com/watch?v=Lxp7147emnM)
  - [The Docs](https://expressjs.com/en/guide/routing.html)

## Best Practices

- `config` file: [how to](https://goenning.net/2016/05/13/how-i-manage-application-configuration-with-nodejs/)

## Deployment

**Directly from GitHub**

- [FCC Article](https://www.freecodecamp.org/news/how-to-deploy-a-nodejs-app-to-heroku-from-github-without-installing-heroku-on-your-machine-433bec770efe/)
- [Heroku CI](https://www.heroku.com/continuous-integration)

**From Terminal**

- [Heroku Getting Started](https://devcenter.heroku.com/articles/getting-started-with-nodejs)
- [Scotch Tutorial](https://scotch.io/tutorials/how-to-deploy-a-node-js-app-to-heroku)
- [Heroku devhints](https://devhints.io/heroku)
- [Heroku DevCenter: Node.js Support](https://devcenter.heroku.com/articles/nodejs-support)
- [Heroku DevCenter: Advanced Automation](https://devcenter.heroku.com/articles/multiple-environments#advanced-linking-local-branches-to-remote-apps)

## From Founders and Coders

[Founders and Coders](https://founders-and-coders.gitbook.io/coursebook/) is another open-source course in web development. They have some great resources for learning Node, Express and Web Apps

- [Node.js](https://founders-and-coders.gitbook.io/coursebook/curriculum/node/schedule)
- [REST APIs](https://founders-and-coders.gitbook.io/coursebook/curriculum/rest-apis/schedule)
- [oliverjam](https://github.com/oliverjam?tab=repositories)
  - take a search through Oliver's repositories, worth it

---

## Class Recordings

> - HYF modules are often updated, recordings from past classes may not match this gitbook
> - When sending a PR's with recording links please ...
>   - Indicate which class you were teaching
>   - Which week it was (if the module is more than 1 week)
>   - a helpful title or description
