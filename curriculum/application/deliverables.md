# Deliverables

There are 3 deliverables for the technical assignment:

1. Create a GitHub account with a profile README.
2. Developing an HTML/CSS web page to explain the basics of HTML & CSS. \(developed on Replit\)
3. Explaining how JavaScript variables work, using JavaScript to explain. \(developed in Replit\)

## 1/3: GitHub Profile

Introduce yourself on GitHub by following these steps:

1. [Create a GitHub account](https://www.wikihow.com/Create-an-Account-on-GitHub) that you will use for _everything_ while at HackYourFuture.
   * !!IMPORTANT!! Choose a username that is **similar to your real name**. This username is how the world will find your code … forever!
2. Write a [GitHub Profile README](https://docs.github.com/en/github/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme) to introduce yourself. Make sure your code is clear and easy to read, we will check!

**What are we looking for with this assignment? Why is a profile README so important?** Markdown is simple to learn, so you can focus on the end product without getting too lost. Writing a good profile README shows that you can:

* Write a well-structured document with complete sentences, good grammar and spelling \(**communication is the most basic skill of a good developer**!\)
* Write clean and well-formatted code. We will be looking at your markdown to make sure it’s good!
* Learn a new software and programming language from resources online.

## 2/3: HTML+CSS Web Page

In this step, you’ll build a an HTML/CSS web page to explain how HTML & CSS works. You should explain at least these concepts \(but are free to explore more if you like!\):

* **HTML**:
  * HTML Document structure \(head, body, ...\)
  * Tags \(mention self-closing tags!\)
  * Attributes
  * HTML5 Semantic elements
* **CSS**:
  * inline vs. internal vs. external CSS
  * Selectors: type vs. class vs. id
  * Colors, sizes and fonts
  * Positioning elements

### Getting Started

1. **Go to** [**Replit.com**](https://replit.com/) and sign in using your GitHub account.
2. **Create a** [**new HTML project**](https://replit.com/new/html) **and get started with your first project!**
   * You will share a link to this Replit project in your application.
3. **Study some HTML and CSS on your favorite tutorial site.** There’s no requirement how much you study, what matters is that you build an awesome portfolio.
4. **Build your web page**: You will probably make many changes as you study and build at the same time, that's great! It doesn’t have to be perfect. Your web page should show us that:
   * you understand what you have learned
   * you’re able to create the **layout of a basic website** \(no specific requirements\)
   * you’re able to **apply** _**and**_ **explain new programming concepts**
   * you can write clear, organized code with comments explaining your thoughts

### Project Assessment

Show us that you understand the basics of HTML & CSS

* Include a menu that links to different parts of your page
* Write correct and clean code that is easy to read
* Comment your code to show us your thought process
* Used HTML5 semantic elements when possible
* Added an alt attribute to ALL images
* Remove inline styles, all of your styling should be external in a .css file
* CSS classes have helpful and descriptive names
* Used CSS _classes_ to style your document \(not _ids_!\)

Don't forget to [format](https://studio.code.org/docs/concepts/html/formatting-html/) your code! It should be easy for us to understand your project's structure simply by looking at the code.

## 3/3: Explain Variables

At HYF you will learn that good code should _first_ be understandable to a human, and _second_ to the computer. To show that you have understood the first steps of JavaScript _and_ that you can explain yourself to other developers, you will create a [new Node.js Replit](https://replit.com/new/nodejs) to explain how variables work.

Your code should not be fancy or complicated! Understandable code, helpful logs, clear explanations, and good links and are more important than an impressive program.

Please limit your JavaScript files to use _**only**_ these JS language features. We want to see how much you can do with less:

'use strict';  
 You should write \`'use strict';\` at the top of each file. This will help you catch some mistakes by telling JS to be more ... strict. \`\`\`js 'use strict'; \`\`\`

Comments  
 Comments are code that the computer ignores. They are there only to help other people understand what you wrote. \`\`\`js 'use strict'; /\* block comments can be many lines long - this is - helpful for writing longer explanations or including links - https://www.youtube.com/watch?v=Jvrszgiexg0 \*/ // in-line comments are only one line long // they're helpful to give a short explanation about a couple lines \`\`\`

console.log and strings  
 Strings are any text wrapped in quotes. You can use double quotes \(\`"\`\), single quotes \(\`'\`\) or back-ticks \(\`\\`\`\) to create a string. \`console.log\` lets you print text to the console. The simplest way to do this is writing a string in the parenthesis like so: \`\`\`js 'use strict'; // prints 'hello!' to the console console.log\('hello!'\); // -&gt; 'hello!' // prints 'good bye.' to the console console.log\('good bye.'\); // -&gt; 'good bye.' \`\`\`

variables declared with `let`  
 There are 3 ways to declare a variable in JavaScript: \`let\`, \`const\` and \`var\`. You only need to understand and use \`let\`, you do not need to explain the others or compare them to \`let\`. Try your best to use helpful variable names, this will make your code much easier for others to read! \`\`\`js 'use strict'; /\* there are 4 important words to pay attention to when studying variables: declare: creating a new variable in program memory assign: storing a value in a variable for later initialize: assigning a value to a variable when it is declared read: using a value that is stored in a variable \*/ // declare a variable named \`oneVariable\` and initialize it to 'hello' let oneVariable = 'hello'; // assign a new value to this variable oneVariable = 'hello!'; // read the value stored in \`oneVariable\` and log it to the console console.log\(oneVariable\); // -&gt; 'hello' // declare a variable without initializing it let anotherVariable; // assign a value to this variable anotherVariable = 'good bye'; // read the value and log it to the console console.log\(anotherVariable\); // -&gt; 'good bye' \`\`\` Here are three mistakes you will probably make, can you figure out how to fix them? &gt; Hint: you may want to create a file for each error and explain how to fix them ;\) \`\`\`js 'use strict'; // assigning a value to a variable that has not been declared undeclaredVariable = 'huh?'; // ReferenceError: undeclaredVariable is not defined \`\`\` \`\`\`js 'use strict'; // reading from a variable that has not been declared console.log\(undeclaredVariable\); // ReferenceError: undeclaredVariable is not defined \`\`\` \`\`\`js 'use strict'; let declaredTwice = 'hi'; let declaredTwice = 'bye'; // SyntaxError: Identifier 'declaredTwice' has already been declared \`\`\`

string concatenation  
 You can combine more than one string using \`+\`. \`\`\`js 'use strict'; // combines 'hello' and '!', then prints the new string console.log\('hello' + '!'\); // -&gt; 'hello!' // you can concatenate two strings and assign that to a variable let greeting = 'h' + 'i'; console.log\(greeting\); // -&gt; 'hi' // you can also concatenate strings that are stored in a variable let excitedGreeting = greeting + '!'; console.log\(excitedGreeting\); // -&gt; 'hi!' \`\`\`

And here is a little example to get you started, you can use it or ignore it. Impress us!

```javascript
'use strict';

let word;
word = 'hello';

let punctuation = '?';
punctuation = '!';

let greeting = word + punctuation;
```

