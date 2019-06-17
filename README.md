# Project Overview

In this project you are given a web-based application that reads RSS feeds. The original developer of this application clearly saw the value in testing, they've already included [Jasmine](http://jasmine.github.io/) and even started writing their first test suite! Unfortunately, they decided to move on to start their own company and we're now left with an application with an incomplete test suite. That's where you come in.


## Why this Project?

Testing is an important part of the development process and many organizations practice a standard of development known as "test-driven development." This is when developers write tests first, before they ever start developing their application. All the tests initially fail and then they start writing application code to make these tests pass.

Whether you work in an organization that uses test-driven development or in an organization that uses tests to make sure future feature development doesn't break existing features, it's an important skill to have!


## What will I learn?

You will learn how to use Jasmine to write a number of tests against a pre-existing application. These will test the underlying business logic of the application as well as the event handling and DOM manipulation.


## How will this help my career?

Writing effective tests requires analyzing multiple aspects of an application including the HTML, CSS and JavaScript - an extremely important skill when changing teams or joining a new company.

Good tests give you the ability to quickly analyze whether new code breaks an existing feature within your codebase, without having to manually test all of the functionality.


# Steps

1. After familiarising myself with the project files(index.html, app.js) I started writing the first suite in `feedreader.js` under the Jasmine spec:
    * First test is to loop trought each feed item and make sure that the URL property is defined and it's not empty (using `expect` and `toBeDefined`).
    * Second test is to make sure all feed has a `name` property and it's not empty. I used the same process like in the first test.

2. `Menu test` suite:
    * First test here is to make sure the menu is `toggled` and has initial state of `hidden`.
    * Second is to test whether or not the menu toggles `on` and `off`.
    
3. `Initial Entries` suite:
    * First test here is to load `loadFeed` asynchronous function and test if after completion there is at least one feed in the container
    (Using Jasmine’s `beforeEach()`, everything we include in this function will run before our “expect” test statement. To handle async we use `done()`.)
4. `New Feed Selection` suite:
    * First test ensures when a new feed is loaded by the `loadFeed` function, the feed content changes. We define two an `initial feed entry` and a `new feed entry` variable and compare the content result of the two not to be same.


# Recorces used: 
    * [Jasmine documentation](http://jasmine.github.io)
    * [Udacity Knowledge resorces](https://knowledge.udacity.com/questions/4581)

# Contributing:

This repository is the starter code for _all_ Udacity students. Therefore, we most likely will not accept pull requests.
