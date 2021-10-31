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
  - [Shaun: Running .js files in Node](https://vimeo.com/467644885)
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

### Class 7-8

> [Shaun](https://github.com/badgerbadgerbadgerbadger), [Evan](https://github.com/colevanderswands/)

1. week 1:
   - Part 1: [Node, Web Apps, CLI's, `fs`, `process.argv`, `assert`](https://vimeo.com/414454713)
   - Part 2: [Exercise recap, Project intro](https://vimeo.com/414475261)
   - Wrap-up: [Homework explanation](https://vimeo.com/414475261)
2. week 2:
   - [Part 1](https://vimeo.com/416866173)
   - [Part 2](https://vimeo.com/416889277)
   - [Wrap-up](https://vimeo.com/416906829)
3. week 3:
   - Part 1: [A](https://vimeo.com/417960548), [B](https://vimeo.com/419545487)
   - [Part 2](https://vimeo.com/418360319)
   - [Part 3](https://vimeo.com/418359614)
4. week 4
   - [Part 1](https://vimeo.com/422120045)
   - [Part 2](https://vimeo.com/422148011)
   - [Part 3](https://vimeo.com/422149853)

### Class 9-10

> [Shaun](https://github.com/badgerbadgerbadgerbadger)

1. Week 1
   1. [Node.js 101 & Client/Server](https://vimeo.com/469893530)
   2. [CLI Input with `process.argv`](https://vimeo.com/469895085)
   3. [`assert` & `fs` part 1](https://vimeo.com/469895326)
   4. [`fs` part 2](https://vimeo.com/469895748)
   5. [Entries Manager part 1](https://vimeo.com/469896412)
   6. [Entries Manager part 2 & Project Intro](https://vimeo.com/469897191)
2. Week 2
   1. [Static & Dynamic Data](https://vimeo.com/472210283)
   2. [Express: Params, Body, Queries ...](https://vimeo.com/472211229)
   3. [... Params, Body, Queries](https://vimeo.com/472211640)
   4. [Texidor](https://vimeo.com/472212077)
   5. [Texidor Recap & DIY Wiki](https://vimeo.com/472212418)
3. Week 3
   - [Middleware & Refactoring Servers](https://vimeo.com/488986376)
4. Week 4:
   - [JSON Schemas & Data Validation](https://vimeo.com/488987165)

### Class 11-12

> [Shaun](https://github.com/badgerbadgerbadgerbadger), [Andrej](https://github.com/gajduk), [Hazem](https://github.com/HazemBittar)

1. Week 1: [part 1](https://vimeo.com/515253111), [part 2](https://vimeo.com/515253217), [part 3](https://vimeo.com/515252844), [part 4](https://vimeo.com/515253024)
2. Week 2: [part 1](https://vimeo.com/518077272), [part 2](https://vimeo.com/518093815), [part 3](https://vimeo.com/518093931), [part 4](https://vimeo.com/518094041), [part 5](https://vimeo.com/518094087)
3. Week 3: [Refactoring pt. 1](https://vimeo.com/520916421), [Refactoring pt. 2](https://vimeo.com/520916669), [middleware & error handling](https://vimeo.com/520916816), [homework](https://www.youtube.com/watch?v=Xeb3xWYJUG8)
4. Week 4: [JSON Schemas](https://vimeo.com/523723387), [Schema Validation](https://vimeo.com/523722229), [`t4v` validation library](https://vimeo.com/523722129), [conclusion](https://vimeo.com/523722804)

### Class 13-14

> [Shaun](https://github.com/badgerbadgerbadgerbadger), [Yoshi](https://github.com/yoshimalaise)

1. Week 1:
   1. [Node, NPM, Packages](https://vimeo.com/589765594)
   2. [Express, `localhost`, Request/Response](https://vimeo.com/589767008)
   3. [Dynamic data, File System, Postman](https://vimeo.com/589767381)
   4. [Routing and Parameters, Persistence, Multi-Tier architecture](https://vimeo.com/589767890)
   5. [Slack clone part 1](https://vimeo.com/589768369)
   6. [Slack clone part 2](https://vimeo.com/589768677)
   7. [Monday review session](https://vimeo.com/588250826)
2. Week 2:
   - [part 1](https://vimeo.com/manage/591000419/general)
   - [part 2](https://vimeo.com/manage/591002265/general)
3. Week 3:
   - [part 1](https://vimeo.com/manage/594234206/general)
   - [part 2](https://vimeo.com/manage/594235051/general)
4. [Week 4](https://vimeo.com/manage/598760351/general)
5. [Week 5](https://vimeo.com/manage/604636340/general)

### Class 15

- Week 1: [Developing an Express API - API data to the file system](https://vimeo.com/manage/628980023/general), [mid-week Q/A](https://vimeo.com/manage/631967169/general)
- [Week 2](https://vimeo.com/635168537)
- [Week 3](https://vimeo.com/639075119)
