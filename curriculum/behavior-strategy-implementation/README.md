# 7. Behavior, Strategy, Implementation

[&lt;&lt; Debugging](../debugging.md) \| [Top](../) \| [Separation of Concerns &gt;&gt;](../separation-of-concerns/)

> Be creative while inventing ideas, but be disciplined while implementing them.
>
> * [Amit Kalantri](https://amitkalantri.com/tag/quotes-about-creativity/)

[examples, exercises and guides](https://github.com/HackYourFutureBelgium/behavior-strategy-implementation)

In this module you will explore different ways to break down and solve coding challenges. Along with structured workflows for approaching challenges, you will learn the JavaScript you need to write clear and maintainable solutions including: reading and writing unit tests, formatting+linting, continuous integration and code review.

## Learning Objectives

* 🥚 You can analyze the behavior, strategy and implementation of functions at your level, written by someone else.
* 🥚 You can use `describe`, `it` and `expect` to write unit tests for a working function. You can group your unit tests by _use case_ and can find interesting edge cases.
* 🥚 You can construct solutions to coding challenges given scrambled lines of code.
* 🥚 You understand the Function Design process and can follow the steps to solve simple coding challenges
* 🥚 You can write functions that use higher order functions and built-in JS array methods to solve simple coding challenges.
* 🥚 You can use ES Modules \(`import`/`export`\) to use functions in a different file than they were declared.
* 🐣 You can read MDN documentation to figure out how built-in JS functions & methods are used.
* 🐣 You can find the _prototype chain_ for a value in the debugger's _scopes_ panel.
* 🐣 You can write and contribute code that meets a group's standards.
* 🐣 You can use a checklist to carry out a constructive code review with a classmate.
* 🐥 You can explain the basic principles of _hoisting_ by stepping through a script in the debugger and showing what changes in the _scopes_ panel.
* 🐔 You can validate your function's arguments and throw helpful errors when the arguments are invalid.

## Behavior

What does the function do? What are it’s arguments and it’s return value? How could you use it in a program? Behavior is all about what your function looks like "from the outside", without caring about what is written inside.

Functions behavior is generally described using **documentation**, **unit tests** and **use cases**:

Documentation \(JSDoc comment\) \`\`\`js /\*\* \* Repeats a string a specific number of times. \* \* @param {string} \[text=''\] - The string to repeat. \* @param {number} \[repetitions=1\] - How many times to repeat the string. \* @return {string} The text repeated \`repetition\` number of times. \*/ export const repeatString = \(text = '', repetitions\) =&gt; { // ... an implementation }; \`\`\`

Unit Tests \(pass/fail assertions\) \`\`\`js import { repeatString } from './repeat-string.js'; describe\('repeats a string any number of times:', \(\) =&gt; { describe\('an empty string', \(\) =&gt; { it\('should repeat "" 0 times', \(\) =&gt; { expect\(repeatString\('', 0\)\).toEqual\(''\); }\); it\('should repeat "" 10 times', \(\) =&gt; { expect\(repeatString\('', 10\)\).toEqual\(''\); }\); it\('should repeat "" 100 times', \(\) =&gt; { expect\(repeatString\('', 100\)\).toEqual\(''\); }\); }\); describe\('zero repetitions', \(\) =&gt; { it\('a non-empty string repeated 0 times -&gt; ""', \(\) =&gt; { expect\(repeatString\('asdf', 0\)\).toEqual\(''\); }\); it\('a longer string repeated 0 times -&gt; ""', \(\) =&gt; { expect\(repeatString\('tommywalk', 0\)\).toEqual\(''\); }\); }\); describe\('standard use cases', \(\) =&gt; { it\('should repeat a phrase 3 times', \(\) =&gt; { expect\(repeatString\('go to school', 3\)\).toEqual\( 'go to schoolgo to schoolgo to school' \); }\); it\('should repeat phrases with punctuation', \(\) =&gt; { expect\(repeatString\('"Go!", said Dr. Seuss?', 2\)\).toEqual\( '"Go!", said Dr. Seuss?"Go!", said Dr. Seuss?' \); }\); it\('should repeat strings with special characters', \(\) =&gt; { expect\(repeatString\('\\ \n \t s', 2\)\).toEqual\('\\ \n \t s\\ \n \t s'\); }\); }\); describe\('default values', \(\) =&gt; { it\('should repeat 1 time by default \(second parameter\)', \(\) =&gt; { expect\(repeatString\('asdf'\)\).toEqual\('asdf'\); }\); it\('should repeat "" by default \(first parameter\)', \(\) =&gt; { expect\(repeatString\(\)\).toEqual\(''\); }\); }\); }\); \`\`\`

Use Cases \("real-world" examples\) \`\`\`js import { promptForString } from '../prompts/prompt-for-string.js'; import { promptForNumber } from '../prompts/prompt-for-number.js'; import { repeatString } from '../utils/repeat-string.js'; // repeating a string inside an I/O loop let repeatedText = ''; while \(true\) { const userString = promptForString\('input a string to repeat'\); const userRepetitions = promptForNumber\('how many times to repeat it?'\); const repeatedInput = repeatString\(userString, userRepetitions\); const userConfirmed = confirm\(\`is this correct: "${repeatedInput}"\`\); if \(userConfirmed\) { repeatedText = repeatedInput; break; } } console.log\(repeatedText\); \`\`\` \`\`\`js import { repeatString } from '../utils/repeat-string.js'; // repeating a string from the DOM const userString = document.getElementById\('text-input'\).value; const userRepetitions = document.getElementById\('number-input'\).value; const repeatedInput = repeatString\(userString, userRepetitions\); document.getElementById\('repeated-value-display'\).innerHTML = repeatedInput; \`\`\`

## Strategy

How do you approach solving the problem? There are many strategies to solve the same problem! A way to practice strategy is to think of transforming the arguments to the return value in small steps, _focusing on the data not the code_. This is the realm of flow charts, diagrams, and pseudo-code.

One way to approach strategy is to solve the problem a few different ways by hand, writing what you expect to change in memory at each step. Like if you were the debugger and you couldn't see the source code. Using a pencil and paper is a the best way to go, pick a few test cases and see how you'd solve them manually.

Here are four possible strategies to approach repeating a string. Each one is written as block comment with step-by-step goals focusing on _what_ should happen at each step, not _how_ it will happen. This type of comment is helpful to include in your code:

Iterate until string is long enough \`\`\`js /\* iterating until the new string's length is correct repeatString\(text, repetitions\) =&gt; 1. calculate the final length for the new string 2. create a new string to fill with many text's 3. iterate as long as the new string is too short a. check if the new string is long enough stop if it is, keep going if it is not b. append text to the new c. repeat return: the new repeated string \*/ \`\`\`

Iteration with a stepper variable \`\`\`js /\* iterating over the number of repetitions repeatString\(text, repetitions\) =&gt; 1. create a new string to fill with many text's 2. create a stepper variable, starting at 0 3. iterate from 0 to repetitions a. check if stepper is still less than repetitions keep going if it is, otherwise stop iterating b. append text to the new string c. increment the stepper d. repeat return: the new repeated string \*/ \`\`\`

Recurse with base-case 0 \`\`\`js /\* recursion with base-case 0 i'm using 0 as the base-case because that is the fewest possible repetitions zero repetitions is an empty string, so if repetitions is 0 it will return '' otherwise i'll need to combine the text with a string that has one fewer reptitions repeatString\(text, repetitions\) =&gt; base-case: repetitions is 0 return: an empty string recursive case: repetitions is greater than 0 nextRepetitions = subtract one from repetitions recursedValue = recursively call repeatString with text and nextRepetitions return: text + recursedValue \*/ \`\`\`

Native JS methods \`\`\`js /\* use built-in .js methods repeatString\(text, repetitions\) =&gt; 1. make sure the data is the correct type and format for the method you're using 2. use the method return: the result \*/ \`\`\`

## Implementation

Which language features and which lines of code can you use to make your strategy a reality? There are many ways to code the same strategy. let's look at multiple implementations for each strategy described above, all of these functions will pass the unit tests written in the _Behavior_ section:

### Iterate Until String is Long Enough

While loop, true and break \`\`\`js /\* unconventional and pretty old-school there is a lot of reinventing the wheel while loops are designed to check conditions this is not the simplest solution to read or maintin \*/ export const repeatString = \(text = '', repetitions = 1\) =&gt; { const finalLength = text.length \* repetitions; let repeatedText = ''; while \(true\) { if \(repeatedText.length === finalLength\) { break; } repeatedText = repeatedText + text; } return repeatedText; }; \`\`\`

While loop, logic in head \`\`\`js /\* the cleanest implementation for this strategy it uses the language feature designed for this type of strategy \*/ export const repeatString = \(text = '', repetitions = 1\) =&gt; { const finalLength = text.length \* repetitions; let repeatedText = ''; while \(repeatedText.length

For loop with only a condition check \`\`\`js /\* not the best implementation, it's confusing to read this strategy does not use stepping, and for loops are designed for stepping implementing this strategy with a for loop is putting a square peg in a round hole when someone sees a for loop they expect it to be used like a for loop this implementation uses a for loop like a while loop the computer doesn't care, but the intention is confusing for other devs \*/ export const repeatString = \(text = '', repetitions = 1\) =&gt; { const finalLength = text.length \* repetitions; let repeatedText = ''; for \(; repeatedText.length

### Iteration with Stepper Variable

While loop, true and break \`\`\`js /\* unconventional and pretty old-school there is a lot of reinventing the wheel while loops are designed to check conditions this is not the simplest solution to read or maintain \*/ export const repeatString = \(text = '', repetitions = 1\) =&gt; { let repeatedText = ''; let count = 0; while \(true\) { if \(count === repetitions\) { break; } repeatedText += text; count++; } return repeatedText; }; \`\`\`

While loop, condition in head \`\`\`js /\* a better way to user the while loop since the condition is known easier to read and more conventional than the previous implementation maybe you find this easier to read than a for loop \*/ export const repeatString = \(text = '', repetitions = 1\) =&gt; { let repeatedText = ''; let count = 0; while \(count

For loop \`\`\`js /\* the cleanest implementation for this strategy it uses the language feature designed for stepping \*/ export const repeatString = \(text = '', repetitions = 1\) =&gt; { let repeatedText = ''; for \(let count = 0; count

### Recursion with Base-Case 0

Ternary Operator \`\`\`js // in all it's ES6 one-line glory // some people find this easier to read than conditionals export const repeatString = \(text = '', repetitions = 1\) =&gt; repetitions === 0 ? '' : text + repeatString\(text, nextRepetitions - 1\); \`\`\`

Conditional Statement \`\`\`js // good old fashioned conditional blocks // some people find this easier to read than ternaries export const repeatString = \(text = '', repetitions = 1\) =&gt; { if \(repetitions === 0\) { return ''; } else { const nextRepetitions = repetitions - 1; const oneRepetitionShort = repeatString\(text, nextRepetitions\); return text + oneRepetitionShort; } }; \`\`\`

Conditional Statement \(tail-call recursion\) \`\`\`js /\* this implementation is "backwards compatible" that means that it has a different signature \(the extra \`repeated\` parameter\) but can still replace previous implementations without breaking anything \*/ export const repeatString = \(text = '', repetitions = 1, repeated = ''\) =&gt; { if \(repetitions === 0\) { return repeated; } else { const nextRepeated = repeated + text; const nextRepetitions = repetitions - 1; return repeatString\(text, nextRepetitions, nextRepeated\); } }; \`\`\`

### Built-In JS Methods

Sting.prototype.repeat \`\`\`js // short and sweet, no room for mistakes export const repeatString = \(text = '', repetitions = 1\) =&gt; text.repeat\(repetitions\); \`\`\`

Array.prototype.fill

```javascript
// less clear and more complex, but still pretty clear to read
export const repeatString = (text = '', repetitions = 1) => {
  const oneEntryPerRepetition = Array(repetitions).fill(text);
  const repeatedString = oneEntryPerRepetition.join('');
  return repeatedString;
};
```

## Learning Objectives

> this module stays close to the code, so to speak. It does not intend to go towards abstracting algorithms, complexity or other CSy concepts.
>
> the objective is that students are prepared to collaborate on a shared code base by learning to write clean and language-specific code, and decipher then improve less clean code.
>
> "at their level" and "level-appropriate" is not yet well-defined. It's some combination of language features used, complexity of strategy, and complexity of the problem. for most objectives it _does not_ require that they could write the solution themselves.

* 🥚 **Analyzing Functions**: A student can analyze a function written at or near their level. This includes:
  * _Behavior_: How would you document the function, what test cases does it pass, and how might you use it in a program
  * _Strategy_: Roughly, how could you translate this solution to pseudo-code.
  * _Implementation_: What language features were used, and what are some alternate language features that could be used
* 🥚 **Testing Existing Functions**: A student can write unit tests for a working function using the `describe`/`it`/`expect(_).toEqual(_)` syntax. This includes grouping test cases into logical test suites.
* 🥚 **Function Design**: A student can explain the function-design process and can successfully apply it to write 2+ solutions matching the behavior of a given function \(assuming the behavior is at their level\). The solutions do not need to implement different strategies, consider edge cases, or check for invalid arguments.
* 🥚 **Generating Documentation**: A student can write a correct JSDoc for their functions and use a provided script to generate markdown documentation in a separate file.
* 🐣 **Array Strategies**: A student can determine which of the primary array strategies \(`map`, `filter`, `reduce`, `every`, `some`\) are helpful for a specific problem at their level.
* 🐣 **Higher-Order Functions in Array Methods**: A student can explain how a higher order function works, and write a callback for use in the primary array methods \(for a problem at their level\).
* 🐣 **Test-Driven Development**: A student can write basic unit tests for a problem they understand without having a solution to validate their tests. They can use their tests as a guide to develop a solution. They do not need to consider edge cases or invalid arguments.
* 🐣 **Testing Side-Effects**: A student can write a suite of unit tests to ensure that; 1\) a function does not modify it's reference-type arguments, 2\) the function returns a new array/object.
* 🐣 **Linting**: A student understands the purpose of linting \(static analysis\) and can successfully fix linting mistakes in a given function.
* 🐣 **ECMAScript Modules**: A student can use `export const functionName = () => {};` and `import { functionName } from './file-name.js'` syntax to separate unit tests from the function definition.
* 🐣 **Continuous Integration**: A student can check CI scripts locally to ensure their code will pass CI checks when it is pushed.
* 🐣 **Code Review**: A student can use a provided checklist and passing/failing CI checks to review a classmate's function \(given the solution is at their level\).
* 🐥 **Testing Edge Cases**: A student can identify and write unit tests for tricky edge cases.
* 🐥 **Writing Guards**: A student can write guards for their function parameters that enforce the function's documented parameter types.
* 🐥 **Testing Guards**: A student can use `expect(() => _).toThrow(_)` to unit-test their guards' error type and message.
* 🐥 **Hoisting**: A student can find hoisted functions and variables in the browser's debugger and explain the semantics of hoisting.
* 🐥 **Prototype Delegation**: A student can inspect a JS value in the browser's debugger/console and explain how to find which methods are available for that value.

