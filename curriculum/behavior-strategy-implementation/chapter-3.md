## Week 3

Code Quality! Code Review!

In the last two weeks you've explored all the different ways people solve coding problems, and discovered many of the strange things JavaScript is capable of. This week it's time to focus in on best practices. You will learn how to use automated tools to check your own code's quality, and a check-list to review each other's code:

- **Generated Documentation**: Use [jsdoc-to-markdown](https://github.com/jsdoc2md/jsdoc-to-markdown/) to convert your JSDoc comments into markdown documentation in a README file.
- **Testing**: Use unit tests to show that your code does what you think it does.
- **Formatting**: Use [Prettier](https://prettier.io/) to format your code, making sure that all the code in your group's repository is formatted the same way and is easy to read.
- **Linting**: Just because your code runs doesn't mean it's good! Use [ESLint](https://eslint.org/) to make sure that everyone's code is easy to read, avoids common mistakes, and uses a consistent style. Linting will be the trickiest thing to get used to, it's basically a loud voice saying "_NO!_" to all sorts of things in your code. But it's for your own good, linting makes it easier to write quality code and to collaborate on a group exercise.
- **Code Review**: Not everything can be automated, you will also learn how to review each other's code. This week's group exercise comes with at Pull Request template that has a big checklist of everything you need to check. Before you can merge any pull request all of the boxes need to be checked. Also a little annoying at first, but better in the long run.

<details>
<summary>expand/collapse</summary>
<br>

### Before Class

Clone the [practice-code-review](https://github.com/hackyourfuturebelgium/practice-code-review) repository and spend some time studying the example solution. You will want to:

- install the repository dependencies
- practice running the solution and the tests
- practice running the code quality scripts

### During Class

#### Before Break

What is Linting? Why is it important?

- **All together**: Fix a few style mistakes in the [./linting](./linting) exercises
- **In small groups**: take a look through the `practice-code-review` repo one someone's local computer. Can you figure out how to run all the code quality scripts?

#### After Break

What is code review? Why is it important?

- **All together**: Discuss code review, your coach's personal experience, and the [code review checklist](https://github.com/hackyourfuturebelgium/practice-code-review/tree/master/.github/PULL_REQUEST_TEMPLATE/code-review-checklist.md). (PS. GitHub has great tools for reviewing code in a Pull Request)
- **In small groups**: Read through the code review checklist and prepare for the week

### After Class

> group exercises

This week's assignment is a group exercise. Your goal isn't to solve as many problems as possible, it's to solve problems as _well_ as possible. You will put extra time into your solutions to make sure everything is perfect - strategy, formatting, linting, testing, and documentation. It will feel like a whole lot of extra work for only small changes, but this is the way of collaboration! Once you get used to it you will see that clean and consistent code saves you lots of time in the long run.

One person in your group should fork [practice-code-review](https://github.com/hackyourfuturebelgium/practice-code-review), everyone in your group will work from that repository. There is no need to have a plan or a development strategy since you are not building a project - each pull request will be for a stand-alone solution. Practicing code review now will prepare you for the next module when you begin building collaborative JS websites .

```markdown
## Practice Code Review

- [ ] [Repo]()
- [Project Board]()
  - [ ] issues are created with the `new solution` template
  - [ ] issues have a label for their challenge and for their strategy
  - (no need for milestones)
- [Pull Requests]()
  - [ ] every solution is pushed to a separate branch (no pushing to main/master!)
  - [ ] every pull request is created with the code-review template
  - [ ] every pull request is labeled with the challenge and strategy
  - [ ] every box is checked _before_ merging a branch to master/main
- [Retrospective]()

> no need for planning this week. Just open a new issue on the project board each time you start a solution
```

Take a look at these examples/exercises, they will be helpful:

- 🥚 **[./linting](./linting)**: Practice using feedback from ESLint to write code that uses consistent style and best practices.
- 🐣 **[./ecmascript-modules](./ecmascript-modules)**: Learn the first basics of using `import` and `export`. Just enough to complete this module's group exercises.

</details>
<br>

[TOP](#behavior-strategy-implementation)

---
