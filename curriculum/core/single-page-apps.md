# Single Page Apps - 2 wk

> 2 weeks. Find the Module repository [right here](https://github.com/HackYourFutureBelgium/single-page-apps/)

Learn to write web sites that feel like multiple pages, but are really only 1 HTML file a lot of JavaScript! Using _UI components_ and _front-end routing_ you can recreate the experience of many HTML pages while writing cleaner and more maintainable code.

## Pains & Gains

* Managing multiple HTML files can get difficult, especially when they need to have the same navbar or elements. UI Components will allow you to build each page from the same code!
* Deciding which elements to write in your HTML and which to render with views can make your pages complex to design. Make things simpler by rendering everything with JavaScript
* Re-rendering elements in your web page is cool and can make a smooth user interface, but it can be very frustrating for users when they cannot go forwards or backwards in your site. Learn how to use frontend routing so that your site's URL changes when the site is rerendered.

## What you can Build

After this module you will build your entire web pages using only JS and CSS! This may feel like more work at first, but over time you will find that this approach makes it easier to design, test, and maintain your code. \(plus, it's great preparation for learning frontend frameworks later on\).

Your projects will have one main `app.js` file that renders the entire user interface into `<div id="root"></div>`, all the rest of your UI will be created from JS Components. From now on your HTML files will look like this, no more and no less:

```markup
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf8" />
    <title>your project name</title>

    <link href="./public/style.css" rel="stylesheet" />
  </head>

  <body>
    <!-- the logging utilities will be rendered here -->
    <div id="logs"></div>

    <!-- your web page will be rendered into this element -->
    <div id="root"</div>

    <!-- initialize your application -->
    <script type="module" src="./src/init/index.js"></script>

    <!-- initialize the logging button  -->
    <script type="module" src="./lib/log-the-logs.js"></script>
  </body>
</html>
```

## Tech Stack

There isn't much new code in this module, what will change the most is how you plan and organize your code.

* JavaScript
  * closure
* Libraries
  * [navigo](https://github.com/krasimir/navigo) - frontend routing library

## New Frontiers

Now that you are comfortable planning and developing component-based Single Page Applications, it's time to take a step out of your browser and begin using APIs in ...

