# 6. Debugging

[&lt;&lt; Welcome to JS](../welcome-to-js/README.md) \| [Top](../README.md) \| [Behavior, Strategy, Implementation &gt;&gt;](../behavior-strategy-implementation/README.md)

> If debugging is the process of removing software bugs, then programming must
> be the process of putting them in.
>
> - [Donald Knuth](https://en.wikipedia.org/wiki/Donald_Knuth)

---

[examples, exercises and guides](https://github.com/HackYourFutureBelgium/debugging)

---

## Learning Objectives

> objectives are limited to programs under 40 lines written in the subset of JS covered in `/isolate`

- 🥚 **Stepping Through**: You can pause a script in a step debugger (breakpoints and `debugger` statement), arrange the debugger, collapse extra panels, and step through a script written with Just Enough JS. At each point in execution you can make a prediction of the next line before executing, and can check your prediction using the _scopes_ panel.
- 🥚 **Assertion Testing**: You are familiar with assertions and can use `console.assert` to guide your study of a program.
- 🥚 **Linting**: You can find and fix linting errors in JavaScript programs.
- 🥚 **Naming Variables**: You can analyze a program's variables according to the structured comment, and rename the variables. Your variable names will describe the variable's role in the program and contextualize the variable in the program's domain. This includes deciding whether to use `let` or `const`.
- 🥚 **Logging**: You are capable of tracing specific aspects of a program's execution using `console.log`.
- 🥚 **Program Life Cycle**: You can explain the two phases of a program's life cycle.
- 🥚 **Fixing Errors**: You can use the structured comment to describe an error in your program, and can make several educated guesses at how to fix the error.
- 🥚 **Documenting Functions**: You can demonstrate your understanding of arguments, parameters and return values by writing a JSDoc comment.
- 🐣 **Explicit Coercion**: You is aware of the rules for casting explicitly between types and can complete assertions to describe what value will result, they can have access to the internet and a console.
- 🐣 **Implicit Coercion**: You is aware that operators will implicitly cast it's operands to the same type before operating. They can look or experimentally discover the rules for an operator.
- 🐣 **Statements vs. Expressions**: You can explain the difference between a statement and an expression, and can identify them in a program. This will be very helpful for understanding how the debugger steps, and for ...
- 🐣 **Operator Precedence**: You can refactor an expression with several operators into several statements assigning each step of the expression to a new variable according to the languages rules of operator precedence.111
- 🐣 **Fixing Bugs**: You can use the structured comment to describe and fix a bug in small programs.
- 🐣 **Reference vs. Value**: You can explain how to swap references or values between variables, explain deep vs. strict equality, and compare two objects or arrays.
- 🐣 **Side-Effects**: Given a function that takes an array as an argument you can determine if the function has any side-effects, and can suggest a way to avoid the side-effect.
- 🐣 **Debugging Functions**: You can read input/output assertion tests to understand a function's actual vs. expected behavior, and to correct the function's behavior.
- 🐥 **Sub-Goal Authoring**: Given most of a small program with missing goal, you can write code to implement the missing behavior.
- 🐥 **Hoisting**: You can find hoisted functions and variables in the browser's debugger and explain how hoisting is related to program life-cycle.
- 🐔 **Refactoring Functions**: You can refactor a designated chunk of a program into an empty function body and pass the given assertion tests.
- 🐔 **Reverse-Engineering**: You can write a small program from scratch that matches the behavior of an example program.

---

![Debugging Tactics](./assets/faasandfurious-debugging.png)

- [faasandfurious](https://faasandfurious.com/71)
