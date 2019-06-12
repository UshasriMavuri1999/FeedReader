# FEED READER
## Table of Contents:
-   [Over View](#Over-View)
-   [Instructions](#Instructions)
-   [Why this Project](#Why-this-project)
-   [How to Run](#How-to-Run)
-   [What will I learn](#What-will-I-learn)
-   [How I built](#How-I-built)
-   [How will this help my career](#How-will-this-help-my-career)
-   [Development Strategy](#Development-Strategy)
-   [Contributing](#Contributing)
## Over View

In this project you are given a web-based application that reads RSS feeds. The original developer of this application clearly saw the value in testing, they've already included [Jasmine](http://jasmine.github.io/) and even started writing their first test suite! Unfortunately, they decided to move on to start their own company and we're now left with an application with an incomplete test suite. That's where you come in.



## Instructions

Use this [rubric](https://review.udacity.com/#!/rubrics/18/view) for self-checking your submission. Your project will be evaluated by a Udacity code reviewer according to the `Feed Reader Testing project rubric`.


## Why this Project?

Testing is an important part of the development process and many organizations practice a standard of development known as "test-driven development." This is when developers write tests first, before they ever start developing their application. All the tests initially fail and then they start writing application code to make these tests pass.

Whether you work in an organization that uses test-driven development or in an organization that uses tests to make sure future feature development doesn't break existing features, it's an important skill to have!

## How to Run?

You can download the starter code through either:

-   feedreader project repository on GitHUB: <https://github.com/udacity/frontend-nanodegree-feedreader.git>
-   The Zipped File : <https://github.com/udacity/frontend-nanodegree-feedreader/archive/master.zip>

    After downloading the starter code open index.html in any web browser to run the project.
    Other way to run this project:
    * Open any webserver for chrome(200 Ok)
    * Choose folder where you saved the project folders
    * Copy the URL link there
    * Now you can paste this URL link on any web browser(Chrome, opera). It redirected to index.html file

## What will I learn?

You will learn how to use Jasmine to write a number of tests against a pre-existing application. These will test the underlying business logic of the application as well as the event handling and DOM manipulation.

## How I built?

-   **Step-1:** Added a test that loops through each feed in the allFeeds object and ensures it has a URL defined and that the URL is not empty.
-   **Step-2:** Added a test that loops through each feed in the allFeeds object and ensures it has a name defined and that the name is not empty.
-   **Step-3:** Added a new test suite named `The menu`
-   **Step-4:** Added a test that ensures the menu element is hidden by default and analyzed the HTML and the CSS to determine how we're performing the hiding/showing of the menu               element.
-   **Step-5:** Added a test that ensures the menu changes visibility when the menu icon is clicked. This test should have two expectations: the menu displays when clicked and it hide when clicked again.
-   **Step-6** Added a new test suite named `Initial Entries`
-   **Step-7:** Added a test that ensures when the loadFeed function is called and completes its work, there is at least a single .entry element within the .feed container. loadFeed() is asynchronous so this test will require the use of Jasmine's beforeEach and asynchronous done() function.
-   **Step-8:** Added a new test suite named `New Feed Selection`
-   **Step-9:** Added a test that ensures when a new feed is loaded by the loadFeed function that the content actually changes.

## How will this help my career?

Writing effective tests requires analyzing multiple aspects of an application including the HTML, CSS and JavaScript - an extremely important skill when changing teams or joining a new company.

Good tests give you the ability to quickly analyze whether new code breaks an existing feature within your codebase, without having to manually test all of the functionality.

# Development Strategy

For a refresher (or reference) before you begin writing code, we recommend reviewing the content from [JavaScript Testing](https://www.udacity.com/course/javascript-testing--ud549). Your project will be evaluated by a Udacity code reviewer according to the [Feed Reader Testing project rubric](https://review.udacity.com/#!/rubrics/18/view). Please review for detailed project requirements.

1.  Familiarize yourself with the starter code
    -   Open up `index.html` and review the functionality of the application within your browser
    -   What is all the code in `app.js` doing? Be sure to read all code comments
    -   Check out `style.css`. How is styling applied to the application?
2.  Explore the Jasmine spec file in `feedreader.js`
    -   This is the file in which you'll be writing your tests
    -   Make sure to read all code comments here as well
    -   Review the [Jasmine documentation](http://jasmine.github.io) if needed
3.  Edit the `allFeeds` variable in `app.js` to make the provided test fail
    -   See how Jasmine visualizes this failure in your application
    -   Return the `allFeeds` variable to a passing state after reviewing the failed test
4.  Write a test that loops through each feed in the `allFeeds` object and ensures it has a URL defined _and_ that the URL is not empty
    -   For example, how would you use a `for...of` loop in this test?
5.  Write a test that loops through each feed in the `allFeeds` object and ensures it has a name defined and that the name is not empty
    -   Think about how you wrote the previous test. What are you testing for this time?
6.  Write a new test suite named `"The menu"`
    -   What are you `describe`-ing in this test suite?
7.  Write a test that ensures the menu element is hidden by default
    -   You'll have to analyze the HTML and the CSS to determine how the hiding/showing of the menu element is implemented
    -   What code in `app.js` is directly involved with toggling the menu on and off?
8.  Write a test that ensures the menu changes visibility when the menu icon is clicked. This test should have two expectations: does the menu display itself when clicked, and does it hide when clicked again?
    -   Think about how you wrote the previous test. What is different this time around?
    -   Which clickable element are you checking for?
    -   How do you "simulate" a mouse click that element without actually clicking it?
9.  Write a test suite named `"Initial Entries"`
    -   What are you `describe`-ing in this test suite?
10. Write a test that ensures when the `loadFeed` function is called and completes its work, there is at least a single `.entry` element within the `.feed` container
    -   How does Jasmine's `beforeEach()`function work?
    -   How does the `loadFeed()` function in `app.js` work? Is it synchronous or asynchronous?
11. Write a test suite named `"New Feed Selection"`
    -   What are you `describe`-ing in this test suite?
12. Write a test that ensures when a new feed is loaded by the `loadFeed` function that the content actually changes
    -   How is this test different from the previous test?

Additionally, note that:

-   No test should be dependent on the results of another
-   Callbacks should be used to ensure that feeds are loaded before they are tested
-   Error handling should be implemented for undefined variables and out-of-bound array access
-   When complete, all of your tests should pass

When you're all finished, write a `README` file detailing all steps required to successfully run the application. If you have added additional tests, provide documentation for what these future features are and what the tests are checking for.

# Contributing

This repository is the starter code for _all_ Udacity students. Therefore, we most likely will not accept pull requests.
## Note:
 Maintain the internet connectivity while running the project.
