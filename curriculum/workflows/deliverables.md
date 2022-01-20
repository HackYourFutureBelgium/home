# Deliverables

This module has 3 deliverables. One is a contribution to the class repository, one is a group project to practice collaboration and the other is a group project to practice following a development strategy.

_Writing code is still writing!_

Take the time to proof read and edit your code before sharing it. Your colleagues and your future self will thank you. Practice using the NPM scripts in the starter repository and the VSC plugins you installed with the Precourse to write correct markdown:

- Format your code with Prettier
- Fix any spelling mistakes
- Fix any linting errors
- Preview the rendered Markdown or HTML/CSS, does it look like you wanted?

## 1. Student Bio PR

Write a short bio for yourself using Markdown and add it to your class repository using a Pull Request. Just a little intro so your classmates can get to know you.

1. Fork your class repository to your github account:
   - [The Coding Train](https://www.youtube.com/watch?v=_NrSWLQsDL4&list=PLRqwX-V7Uu6ZF9C0YMKuns9sLDzK6zoiV&index=3)
   - [guides.github.com](https://guides.github.com/activities/forking/)
   - [fork vs. clone](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=20&cad=rja&uact=8&ved=2ahUKEwihx9DwkMrhAhVNbVAKHZ4bCEIQFjATegQIABAB&url=https%3A%2F%2Fgithub.community%2Ft5%2FSupport-Series%2FThe-Difference-Between-Forking-and-Cloning-a-Repository%2Fba-p%2F1372&usg=AOvVaw0PCFTCp62bxxeTPAQgW9h4)
2. Create a new file in the ./student-bios folder _on your fork_:
   - **important**: Use your GitHub username as the name of your file. ie. `colevandersWands.md`
   - Go all out! Take a look at this [markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) and [emojis list](https://gist.github.com/rxaviers/7360908) for inspiration
3. Send a pull request to from your fork to the main class repo, use the
   `student-bio` PR template.
   - [The Coding Train](https://www.youtube.com/watch?v=_NrSWLQsDL4&list=PLRqwX-V7Uu6ZF9C0YMKuns9sLDzK6zoiV&index=3)
   - [github help](https://help.github.com/en/articles/creating-a-pull-request)
   - [github guides](https://guides.github.com/activities/forking/)

### Checklist to paste into your deliverable issue:

```markdown
[my fork](_)

> PS. don't forget to [link your PR to this issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue)!
```

## 2. GitHub Profile README

> use this starter repository: [Markdown template repository](https://github.com/HackYourFutureBelgium/template-markdown)

Using the [Markdown template repository](https://github.com/HackYourFutureBelgium/template-markdown) as a starter, [create a new repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template) on your account named _exactly_ your GitHub user name.

After creating your repository you will need to _clone_ it to your local computer and follow the **Getting Started** instructions in the README. Once you're familiar with the instructions you will need to delete them all to write your README. (no worries, the instructions will always be in the template.)

Writing your profile README is not only about personalizing your GitHub account, it's also a chance for you to practice writing clean code, running NPM scripts, using git, and VSCode. Practicing these skills alone first will make your first group project much easier.

```markdown
- [ ] [profile README repository](https://github.com/_/_)
- [ ] [my account with live README](https://github.com/_)
- I have practiced:
  - [ ] Pulling and pushing
  - [ ] formatting my code: `npm run format`
  - [ ] checking my spelling: `npm run spell-check`
  - [ ] linting my code: `npm run lint:ls` _and_ `npm run lint:md`
```

## 3. Flashcards Repository

Flashcards a great way to learn anything, even programming! We suggest you use the [Leitner System](https://www.youtube.com/watch?v=6S2LJIAydyg) to organize your flashcards and study schedules.

Paper flashcards are of course a great option, but it can be harder to share these with your classmates and sometimes it is nice to have an interactive code snippet in your flashcards. To manage your own Markdown flashcards and study schedule you can fork the [HackYourFutureBelgium/flashcards](https://github.com/hackyourfuturebelgium/flashcards) repository to your GiHub account, then clone it to your computer.

You will be using this through HYF to build your own collection of interactive flashcards. There's some tips for getting started in the repository's README.

## 4. Vocabulary

Make at least 1 issue with a linked PR contributing to the `/vocabulary` folder of your class repo:

- _Labels_: `deliverable`, `vocabulary`
- _milestone_: `workflows`

Careful! Check with your classmates before sending your PR. You should coordinate as a class to make sure everyone isn't adding the same vocab words, and to make sure there aren't more than one documents for the same topic.

And please limit your vocabulary to topics covered in this module. For example vocab related to Git or GitHub are welcome, but vocabulary related to JavaScript is not allowed.

## 5. Group Introduction

> use this starter repository: [Markdown template repository](https://github.com/HackYourFutureBelgium/template-markdown)

Find a time to meet with your study group and build a get-to-know-you repository with one markdown file per person in your group. This doesn't need to be anything fancy. Your focus should be on getting to know each other and learning to work on a shared repository.

When you're ready to start your group repo, create a new issue in the class repo using the `deliverable` template and add the `group` label. Fill out the project's description, list your group members, and paste this checklist into your issue before [adding it to the Class Projects board](https://docs.github.com/en/free-pro-team@latest/github/managing-your-work-on-github/adding-issues-and-pull-requests-to-a-project-board):

> PS. check out other HYF classes for inspiration

### Checklists

- For your group's `deliverable` issue in the class repo:

  ```markdown
  <!-- replace the _ with the correct user name and repo -->

  - [ ] [repo](https://github.com/_/_)
  - [ ] [many small, well-named commits](https://github.com/_/_/commits)
  - [ ] a nice README
  - [ ] one well-named file per person
  - [ ] [one pull requests for each group member](https://github.com/_/_/pulls)
    - [ ] linting checks pass
    - [ ] code review checklist is complete
    - [ ] the reviewer merged the code
  ```

- For your individual PRs in your group repository

  ```markdown
  - Setup: GitHub
    - [ ] created this issue
    - [ ] assigned myself
    - [ ] moved the issue to the project board
  - Setup: local
    - [ ] pulled the most recent code from `main`/`master`
    - [ ] created a new branch for my introduction
  - Writing the content:
    - [ ] added my intro file in `/people` according to group conventions
    - [ ] linked to my file from `/README.md` according to group conventions
  - Before pushing my branch:
    - [ ] formatted the code
    - [ ] fixed all spelling mistakes and added new words to the dictionary
    - [ ] fixed all linting mistakes
  - After pushing my branch:
    - [ ] created a new PR linked to this issue
    - [ ] make sure all of the checks passed
    - [ ] assigned someone to review and merge my PR
  ```

## 6. Planning and Collaborating

> - the HTML & CSS code, and planning documents are in [workflows/project-starter](https://github.com/workflows/tree-master/project-starter)
> - use this template repo: [HTML & CSS template repository](https://github.com/HackYourFutureBelgium/template-html-css)

This project is to rebuild the HTML & CSS from `/project-starter` in a new repository as a group using Pull Requests. All the planning documents except _User Personas_ are already provided for you in `/project-starter`.

You _will not_ be planning a new webiste, and you _will not_ be writing your own code. Your main focus should be the steps in [Planning and Collaborating](https://home.hackyourfuture.be/students/planning-and-collaborating), Git/GitHub workflows, and code review using a checklist.

In the next module you’ll get the chance to be creative and plan full websites from scratch. for now you should just focus on learning the workflows and processes so you’re more free to be creative in the future.

```markdown
- [ ] [repo](https://github.com/_/_) (with a complete README)
- [ ] [live demo](https://_.github.io/_)
- [/planning](https://github.com/_/_/tree/master/planning)
  - [ ] communication plan
  - [ ] constraints
  - [ ] user personas (_you need to write this!_)
  - [ ] backlog
  - [ ] design
  - [ ] development strategy
  - [ ] retrospective
- [ ] [project board](https://github.com/_/_/projects/1)
```
