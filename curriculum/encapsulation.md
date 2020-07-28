# Encapsulation

> Find the Module repository [right here]() (coming soon)

Up until now you've been learning how to break your code into more, smaller pieces based on the role it plays in your application.  Learning to do this is a critical skill but as you've probably noticed, it is difficult to manage projects when your code is in so spread out.

If the last modules were about breaking your projects down, then this module is about building them up.

__Encapsulation__ is the idea of grouping together your data with the functions that use it. That's it! (for now :)  There are many ways to achieve this, but the end result is code that is easier to understand and nicer work with.

Heads up!  In this module you'll be encountering some of the most important (and most challenging!) aspects of the JavaScript language: closure, `this` & inheritance.  These are all features of JS that allow you to encapsulate and re-use your code.

Along the way you will get your first introduction to one of the main programming paradigms in JS: _object oriented programming_.  At their simplest level, programming paradigms are just different answers to the same question "How will I group my data and my functions?".

## Pains & Gains

* The way you have organized your code so far was helpful for your first small projects.  But as your projects grew, your code became more and more scattered.  To make a change to one functionality (user story) you needed change code in at least 2-3 different files. Learn a more _scalable_ way to organize your code by _encapsulating_ all code related to one functionality into a single object or function.
* Updating your user interfaces with DOM manipulation can be messy and difficult to debug.  Learn how to build your user interfaces with modular, reusable & testable _DOM components_.
* So far you have learned about 3 types of variables inside of your functions: _arguments_, _local variables_ and _global variables_.  Using global variables in your handlers to update state, call logic, or modify the DOM is not generally a good practice.  JavaScript has important way to access values from inside a function call that will allow you to avoid accessing global scope:  `this`.

## What you can Build

Build more complex web pages that use `this` (objects) to encapsulate related code into a single "thing".  With this technique you will be able to build bigger apps by making smaller ones and gluing them together!

## Tech Stack

What's new in this module?

* JavaScript
  * `this`: context vs. bind vs. call/apply
  * Inheritance: Constructor Functions, Classes, `Object.create`


## New Frontiers

You have mastered the art of application design!  Or at least taken your first steps :hatching_chick:.

Now that you are comfortable planning, debugging and building apps to manage hard-coded or user-provided data, it's time to take the training wheels and start consuming ...


