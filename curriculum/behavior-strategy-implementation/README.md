# 7. Behavior, Strategy, Implementation

[&lt;&lt; Debugging](../debugging/README.md) \| [Top](../README.md) \| [Separation of Concerns &gt;&gt;](../separation-of-concerns/README.md)

> Be creative while inventing ideas, but be disciplined while implementing them.
>
> - [Amit Kalantri](https://amitkalantri.com/tag/quotes-about-creativity/)

---

[examples, exercises and guides](https://github.com/HackYourFutureBelgium/behavior-strategy-implementation)

---

In this module you will explore different ways to break down and solve coding challenges. Along with structured workflows for approaching challenges, you will learn the JavaScript you need to write clear and maintainable solutions including: reading and writing unit tests, formatting+linting, continuous integration and code review.

## Learning Objectives

<!--

  this module stays close to the code, so to speak. It does not intend to go towards abstracting algorithms, complexity or other CSy concepts.

  the objective is that students are prepared to collaborate on a shared code base by learning to write clean and language-specific code, and decipher then improve less clean code.

  "at your level" and "level-appropriate" is not yet well-defined. It's some combination of language features used, complexity of strategy, and complexity of the problem. for most objectives it _does not_ require that they could write the solution themselves.

-->

- 🥚 **Analyzing Functions**: You can analyze a function written at or near your level. This includes:
  - _Behavior_: How would you document the function, what test cases does it pass, and how might you use it in a program
  - _Strategy_: Roughly, how could you translate this solution to pseudo-code.
  - _Implementation_: What language features were used, and what are some alternate language features that could be used
- 🥚 **Testing Existing Functions**: You can write unit tests for a working function using the `describe`/`it`/`expect(_).toEqual(_)` syntax. This includes grouping test cases into logical test suites.
- 🥚 **Function Design**: You can explain the function-design process and can successfully apply it to write 2+ solutions matching the behavior of a given function \(assuming the behavior is at your level\). The solutions do not need to implement different strategies, consider edge cases, or check for invalid arguments.
- 🥚 **Generating Documentation**: You can write a correct JSDoc for your functions and use a provided script to generate markdown documentation in a separate file.
- 🐣 **Declarative Programming**: You can explain how _Declarative Programming_ is different from _Imperative_ programming, and can tell which paradigm is used in a program. You can also use built-in JS methods to write Declarative solutions to simple coding challenges.
- 🐣 **Array Strategies**: You can determine which of the primary array strategies \(`map`, `filter`, `reduce`, `every`, `some`\) are helpful for a specific problem at your level.
- 🐣 **Higher-Order Functions in Array Methods**: You can explain how a higher order function works, and write a callback for use in the primary array methods \(for a problem at your level\).
- 🐣 **Prototype Delegation**: You can inspect a JS value in the browser's debugger/console and explain how to find which methods are available for that value.
- 🐣 **Nested Data**: Given a nested data structure containing arrays, objects and primitive values, you can 1\) access a given value 2\) update a given entry 3\) filter the data
- 🐣 **Test-Driven Development**: You can write basic unit tests for a problem you understand without having a solution to validate your tests. You can use your tests as a guide to develop a solution. You do not need to consider edge cases or invalid arguments.
- 🐣 **Testing Side-Effects**: You can write a suite of unit tests to ensure that; 1\) a function does not modify it's reference-type arguments, 2\) the function returns a new array/object.
- 🐣 **ECMAScript Modules**: You can use `export const functionName = () => {};` and `import { functionName } from './file-name.js'` syntax to separate unit tests from the function definition.
- 🐣 **Continuous Integration**: You can check CI scripts locally to ensure your code will pass CI checks when it is pushed, and can read CI results when conducting a code review.
- 🐣 **Code Review**: You can use a provided checklist and passing/failing CI checks to review a classmate's function \(given the solution is at your level\).
- 🐥 **Code Coverage**: You can explain what code coverage is, why it's important, and can write unit tests for a code challenge with 100% coverage.
- 🐥 **Testing Edge Cases**: You can identify and write unit tests for tricky edge cases.
- 🐔 **Writing Guards**: You can write guards for your function parameters that enforce the function's documented parameter types.
- 🐔 **Testing Guards**: You can use `expect(() => _).toThrow(_)` to unit-test your guards' error type and message.

---

## Behavior

What does the function do? What are it’s arguments and it’s return value? How could you use it in a program? Behavior is all about what your function looks like "from the outside", without caring about what is written inside.

Functions behavior is generally described using **documentation**, **unit tests** and **use cases**:

### Documentation (JSDoc comment)

```js
/**
 * repeats a string a specific number of times
 * @param {string} [text=''] - the string to repeat. defaults to empty string
 * @param {number} [repetitions=1] - how many times to repeat. defaults to 1
 *  repetitions cannot be negative, and must be an integer
 * @return {string} the text repeated as many times as repetitions
 */
```

### Unit Tests (pass/fail assertions)

```js
describe('repeats a string any number of times:', () => {
  describe('an empty string', () => {
    it('should repeat "" 0 times', () => {
      expect(repeatString('', 0)).toEqual('');
    });
    it('should repeat "" 10 times', () => {
      expect(repeatString('', 10)).toEqual('');
    });
    it('should repeat "" 100 times', () => {
      expect(repeatString('', 100)).toEqual('');
    });
  });
  describe('zero repetitions', () => {
    it('a non-empty string repeated 0 times -> ""', () => {
      expect(repeatString('asdf', 0)).toEqual('');
    });
    it('a longer string repeated 0 times -> ""', () => {
      expect(repeatString('tommywalk', 0)).toEqual('');
    });
  });
  describe('standard use cases', () => {
    it('should repeat a phrase 3 times', () => {
      expect(repeatString('go to school', 3)).toEqual(
        'go to schoolgo to schoolgo to school'
      );
    });
    it('should repeat phrases with punctuation', () => {
      expect(repeatString('"Go!", said Dr. Seuss?', 2)).toEqual(
        '"Go!", said Dr. Seuss?"Go!", said Dr. Seuss?'
      );
    });
    it('should repeat strings with special characters', () => {
      expect(repeatString('\\ \n \t s', 2)).toEqual('\\ \n \t s\\ \n \t s');
    });
  });
  describe('default values', () => {
    it('should repeat 1 time by default (second parameter)', () => {
      expect(repeatString('asdf')).toEqual('asdf');
    });
    it('should repeat "" by default (first parameter)', () => {
      expect(repeatString()).toEqual('');
    });
  });
});
```

### Use Cases ("real-world" examples)

```js
// repeating a string inside an I/O loop
let repeatedText = '';
while (true) {
  const userString = promptForSomething('input a string to repeat');
  const userRepetitions = promptForNumber('how many times to repeat it?');
  const repeatedInput = repeatString(userString, userRepetitions);
  const userConfirmed = confirm(`is this correct: "${repeatedInput}"`);
  if (userConfirmed) {
    repeatedText = repeatedInput;
    break;
  }
}
console.log(repeatedText);
```

```js
// repeating a string from the DOM
const userString = document.getElementById('text-input').value;
const userRepetitions = document.getElementById('number-input').value;
const repeatedInput = repeatString(userString, userRepetitions);
document.getElementById('repeated-value-display').innerHTML = repeatedInput;
```

## Strategy

How do you approach solving the problem? There are many strategies to solve the same problem! A way to practice strategy is to think of transforming the arguments to the return value in small steps, _focusing on the data not the code_. This is the realm of flow charts, diagrams, and pseudo-code.

One way to approach strategy is to solve the problem a few different ways by hand, writing what you expect to change in memory at each step. Like if you were the debugger and you couldn't see the source code. Using a pencil and paper is a the best way to go, pick a few test cases and see how you'd solve them manually.

Here are four possible strategies to approach repeating a string. Each one is written as block comment with step-by-step goals focusing on _what_ should happen at each step, not _how_ it will happen. This type of comment is helpful to include in your code:

### Iterate until string is long enough

```js
/* iterating until the new string's length is correct

  repeatString(text, repetitions) =>
    1. calculate the final length for the new string
    2. create a new string to fill with many text's
    3. iterate as long as the new string is too short
      a. check if the new string is long enough
        stop if it is, keep going if it is not
      b. append text to the new
      c. repeat
    return: the new repeated string

*/
```

### Iteration with a stepper variable

```js
/* iterating over the number of repetitions

  repeatString(text, repetitions) =>
    1. create a new string to fill with many text's
    2. create a stepper variable, starting at 0
    3. iterate from 0 to repetitions
      a. check if stepper is still less than repetitions
        keep going if it is, otherwise stop iterating
      b. append text to the new string
      c. increment the stepper
      d. repeat
    return: the new repeated string

*/
```

### Recurse with base-case 0

```js
/* recursion with base-case 0

  i'm using 0 as the base-case because that is the fewest possible repetitions
  zero repetitions is an empty string, so if repetitions is 0 it will return ''

  otherwise i'll need to combine the text with a string that has one fewer reptitions

  repeatString(text, repetitions) =>
    base-case: repetitions is 0
      return: an empty string
    recursive case: repetitions is greater than 0
      nextRepetitions = subtract one from repetitions
      recursedValue = recursively call repeatString with text and nextRepetitions
      return: text + recursedValue

*/
```

### Native JS methods

```js
/* use built-in .js methods

  repeatString(text, repetitions) =>
    1. make sure the data is the correct type and format for the method you're using
    2. use the method
    return: the result

*/
```

## Implementation

Which language features and which lines of code can you use to make your strategy a reality? There are many ways to code the same strategy. let's look at multiple implementations for each strategy described above, all of these functions will pass the unit tests written in the _Behavior_ section:

### Iterate Until String is Long Enough

#### While loop, true and break

```js
/* unconventional and pretty old-school
  there is a lot of reinventing the wheel
  while loops are designed to check conditions
  this is not the simplest solution to read or maintin
*/
const repeatString = (text = '', repetitions = 1) => {
  const finalLength = text.length * repetitions;
  let repeatedText = '';
  while (true) {
    if (repeatedText.length === finalLength) {
      break;
    }
    repeatedText = repeatedText + text;
  }
  return repeatedText;
};
```

#### While loop, logic in head

```js
/* the cleanest implementation for this strategy
  it uses the language feature designed for this type of strategy
*/
const repeatString = (text = '', repetitions = 1) => {
  const finalLength = text.length * repetitions;
  let repeatedText = '';
  while (repeatedText.length < finalLength) {
    repeatedText += text;
  }
  return repeatedText;
};
```

#### For loop with only a condition check

```js
/* not the best implementation, it's confusing to read
  this strategy does not use stepping, and for loops are designed for stepping
  implementing this strategy with a for loop is putting a square peg in a round hole

  when someone sees a for loop they expect it to be used like a for loop
  this implementation uses a for loop like a while loop
  the computer doesn't care, but the intention is confusing for other devs
*/
const repeatString = (text = '', repetitions = 1) => {
  const finalLength = text.length * repetitions;
  let repeatedText = '';
  for (; repeatedText.length < finalLength; ) {
    repeatedText += text;
  }
  return repeatedText;
};
```

### Iteration with Stepper Variable

#### While loop, true and break

```js
/* unconventional and pretty old-school
  there is a lot of reinventing the wheel
  while loops are designed to check conditions
  this is not the simplest solution to read or maintain
*/
const repeatString = (text = '', repetitions = 1) => {
  let repeatedText = '';
  let count = 0;
  while (true) {
    if (count === repetitions) {
      break;
    }
    repeatedText += text;
    count++;
  }
  return repeatedText;
};
```

#### While loop, condition in head

```js
/* a better way to user the while loop since the condition is known
  easier to read and more conventional than the previous implementation
  maybe you find this easier to read than a for loop
*/
const repeatString = (text = '', repetitions = 1) => {
  let repeatedText = '';
  let count = 0;
  while (count < repetitions) {
    repeatedText = repeatedText + text;
    count++;
  }
  return repeatedText;
};
```

#### For loop

```js
/* the cleanest implementation for this strategy
  it uses the language feature designed for stepping
*/
const repeatString = (text = '', repetitions = 1) => {
  let repeatedText = '';
  for (let count = 0; count < repetitions; count++) {
    repeatedText += text;
  }
  return repeatedText;
};
```

### Recursion with Base-Case 0

#### Ternary Operator

```js
// in all it's ES6 one-line glory
// some people find this easier to read than conditionals
const repeatString = (text = '', repetitions = 1) =>
  repetitions === 0 ? '' : text + repeatString(text, nextRepetitions - 1);
```

#### Conditional Statement

```js
// good old fashioned conditional blocks
// some people find this easier to read than ternaries
const repeatString = (text = '', repetitions = 1) => {
  if (repetitions === 0) {
    return '';
  } else {
    const nextRepetitions = repetitions - 1;
    const oneRepetitionShort = repeatString(text, nextRepetitions);
    return text + oneRepetitionShort;
  }
};
```

#### Conditional Statement (tail-call recursion)

```js
/* this implementation is "backwards compatible"
  that means that it has a different signature (the extra `repeated` parameter)
  but can still replace previous implementations without breaking anything
*/
const repeatString = (text = '', repetitions = 1, repeated = '') => {
  if (repetitions === 0) {
    return repeated;
  } else {
    const nextRepeated = repeated + text;
    const nextRepetitions = repetitions - 1;
    return repeatString(text, nextRepetitions, nextRepeated);
  }
};
```

### Built-In JS Methods

#### Sting.prototype.repeat

```js
// short and sweet, no room for mistakes
const repeatString = (text = '', repetitions = 1) => text.repeat(repetitions);
```

#### Array.prototype.fill

```js
// less clear and more complex, but still pretty clear to read
const repeatString = (text = '', repetitions = 1) => {
  const oneEntryPerRepetition = Array(repetitions).fill(text);
  const repeatedString = oneEntryPerRepetition.join('');
  return repeatedString;
};
```
