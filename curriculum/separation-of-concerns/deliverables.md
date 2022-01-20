# Deliverables

This module has 2 projects, one individual and one group.

Projects in this module will be more challenging than in the last modules, adding even a little interactivity into a website will make things much more complicated! To help you deal with this complexity you will practice separating and organizing your JavaScript code into different files based on what role it plays in your application.

- **Interactive UI**

  You will learn how to create interactive User Interfaces by reading and writing from the DOM:

  - Users will pass input to your programs directly from the UI (no more `prompt`)
  - Users will see results displayed directly in the UI (no more `alert`)

  Projects in this module will not include full DOM manipulation, you'll learn that in the next module. This module's projects will be limited to reading/writing `.innerHTML` & `.value`.

- **Decoupled Code**

  In this module you will learn how to completely separate your JavaScript from your user interface. You will be using `.getElementById` and `.addEventListener` instead of the `onclick` attribute.

  When using `onclick`, you need to write some JavaScript in your HTML - this is not a good practice because your UI and JavaScript are too interdependent. Using HTML `id`s and JavaScript _event listeners_ you can **decouple** your User Interface from the program utils.

- **DOM Event Listeners**

  Web development is fundamentally _event driven_, this means things don't happen until a something else happens. In your previous projects the `prompt` didn't appear until the user clicked a button and a prompt appeared. You've probably noticed by now that this is a limiting way to write your programs. It's hard to gather interesting data from a user, and impossible to display it in a nice way.

  You will learn how to use _DOM events_ to interact with users and to read more interesting data than just a few words or numbers. Things like mouse movements, the colors on a screen, and much more.

- **Separating your Concerns**

  A working project is not enough! For projects in this module we will expect you to turn in code that is well organized in different files based on it's role. The first week's project will come with some starter-code to help you get used to the folder structure we expect.

- **Development Strategy**

  Just like in the previous module, you will be expected to explain your development strategy in a separate file called `development-strategy.md`. Projects involving JavaScript are naturally more complicated than projects with only HTML and CSS, for this reason you will need to have more types of task (`type: _`) in your `development-strategy`.

- **Git Branching**

  In this module’s project you have many more files and folders, and you’re learning how to break a single feature into more smaller pieces. To implement a single user story you will need HTML, CSS, data, event listener(s), handler(s) and possibly a utils function or a procedure. All of these smaller tasks are pull together into one user story.

  So a PR for one user story may have changes in many folders and files. At first this will feel like more work than necessary, but after a while you will start to see how this way of working makes larger projects easier to understand.

Good luck!

---

## Word List

> [word-list starter](https://github.com/HackYourFutureBelgium/word-list) - individual, due before the 3rd lesson

This week's assignment is for learning how to work on a multi-file project. You will be using this project structure for the next few modules, so no worries if you don't understand everything right away. There's still plenty of time to understand.

There's only about 15-30 lines of JavaScript you need to write. That might not sound like it may not sound like a lot, but it will take some study to figure out what exactly to write where.

And the starter page is pretty ugly. Feel free to improve the HTML and CSS as much as you like! \(just be careful not to break the id's ;\)

```markdown
- [ ] [repo](https://github.com/_/_) (with a complete README)
- [ ] [live demo](https://_.github.io/_)
- [ ] [Docs](https://github.com/_/_/tree/_/DOCS.md)
- [/planning](https://github.com/_/_/tree/_/planning)
  - [ ] constraints
  - [ ] backlog
  - [ ] wireframe
  - [ ] development strategy
  - [ ] retrospective
- [ ] [project board](https://github.com/_/_/projects/1)
```

---

## A List

> [separation-of-concerns-starter](https://github.com/HackYourFutureBelgium/separation-of-concerns-starter) - group project. make it as far as you can, planning is more important than finishing

This week you and your group will build a small project from scratch using the [separation-of-concerns-starter](https://github.com/HackYourFutureBelgium/separation-of-concerns-starter). Here are some possible user stories to get you started:

- A user can see all the items in their list
- A user can add a new item to their list
- A user can remove any item from their list
- A user can edit the description of each item in their list
- A user can mark an item as "done" or "not done"

### Checklist

```markdown
- [ ] [repo](https://github.com/_/_) (with a complete README)
- [ ] [live demo](https://_.github.io/_)
- [/planning](https://github.com/_/_/tree/master/planning)
  - [ ] communication plan
  - [ ] constraints
  - [ ] backlog
  - [ ] wireframe
  - [ ] development strategy
  - [ ] retrospective
- [ ] [project board](https://github.com/_/_/projects/1)
```
