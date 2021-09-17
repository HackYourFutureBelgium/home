## Week 1

The best problem solvers don't start from nothing, they've seen many similar problems before and have learned to adapt other people's code to fit their programs.

This week take your first step to becoming an expert problem solver by studying the many ways people before you have solved common problems.

<details>
<summary>expand/collapse</summary>
<br>

### Before Class

- Fork [solution-write-ups](https://github.com/HackYourFutureBelgium/solution-write-ups)
  - Read through the README, this will be your main exercise for the week.
  - Follow the instructions in **Getting Started** to locally set up your repository.
  - Practice running the `sandbox.test.js` file in the example write-up, in VSCode and the browser. (instructions in **Getting Started**)
- Read through [./about-testing/examples](./about-testing/examples) to be familiar with the syntax for `describe`, `it`, and `expect`
- Create an account on [Edabit](https://edabit.com)

### During Class

In class you will practice writing tests and analyzing solutions using a challenge from [Edabit](https://edabit.com/):

- [Add up the Numbers from a Single Number](https://edabit.com/challenge/4gzDuDkompAqujpRi)

#### Before Break

Description, Syntax, Test Cases and Use Cases.

- All together:
  - look through the examples at the beginning of this README. What is behavior, strategy and implementation?
  - go over the README from [solution-write-ups](https://github.com/HackYourFutureBelgium/solution-write-ups)
  - read through the first 4 sections in the example from [solution-write-ups](https://github.com/HackYourFutureBelgium/solution-write-ups)
- In small groups:
  - Complete the first 4 sections of the writeup for `Add up the Numbers ...`
  - You can use the most popular solution solution by **\_sir** to write your tests:
    ```js
    function addUp(num) {
      return (num * (num + 1)) / 2;
    }
    ```

#### After Break

Strategy, Implementation and Possible Refactors.

- All together:
  - read through the rest of the example in [solution-write-ups](https://github.com/HackYourFutureBelgium/solution-write-ups)
- In small groups:

  - practice writing up 2-3 solutions to the `Add up the Numbers ...` challenge (be sure to test them all!)
  - <details><summary>here's a few suggestions to study:</summary>

    ```js
    // Gabriel
    function addUp(num) {
      let sum = 0;
      for (let i = 1; i <= num; i++) {
        sum += i;
      }
      return sum;
    }

    // 범두
    function addUp(num) {
      var a = 0;
      for (var i = num; i > 0; i--) {
        a += i;
      }
      return a;
    }

    // doodledob
    function addUp(num) {
      x = 0;
      while (num >= 0) {
        x += num;
        num--;
      }
      return x;
    }

    // _sir
    function addUp(num) {
      return (num * (num + 1)) / 2;
    }
    ```

    </details>

### After Class

Take your time this week to explore other people's code. In the past modules you've studied only a small part of what JS, now you're in the wild! You'll come across all sorts of JS features and new coding styles.

Complete as many write-ups as you can. No need to rush ahead! Take your time studying solutions at your level. It's more helpful to study a variety of solutions than to study a few hard ones:

- **[Solution Write-Ups](https://github.com/HackYourFutureBelgium/solution-write-ups)**

Learning to read MDN Documentation will help you understand how JS works, and help you do a good write-up:

- [MDN Documentation](#mdn-documentation)

Practice reconstructing different solutions to the same coding challenge:

- 🐣 **[./parsons-problems](./parsons-problems)**

These exercises will help you understand test cases, and be important for next week:

- 🐣 **[./about-testing](./about-testing)**

Here's some important JS concepts you should start learning about:

- 🥚 **[./implicit-return](./implicit-return)**: just a different way to write functions
- 🐣 **[./array-methods](./array-methods)**: +1
- 🐣 **[./hoisting](./hoisting)**: you _do not_ need to master this! but it will help you understand what's happening in the debugger, some strange bugs, and how `let`/`const` & `() => {}` are different from `var` and `function () {}`
- 🐥 **[./prototype-delegation](./prototype-delegation)**: you _do not_ need to master this! but it will help understand what you see in the debugger, where methods come from, and how to read MDN documentation.

</details>
<br>

[TOP](#behavior-strategy-implementation)

---
