# UI testing

## What To Do in Lab
1. Read over the following introduction. You should have seen Selenium/UI testing in SENG 275. 

2. Then copy the repo using the Classroom invite (one person can do it for the group to follow) and then get it to reproduce the test. Make sure your team understands a) how to configure Selenium and the web driver; b) how to run the tests (in this case, with `Mocha`); c) the concept of locating web elements with selectors.

3. Then decide on the GUI testing approach you will use in your assignment 5 testing. Your team should have a completed GUI test plan mapped to user stories by the end of the lab.

## Overview
We could (and SHOULD) do usability testing with real users, [focus](https://www.youtube.com/watch?v=8YDpvMYk5jA) [groups](https://www.youtube.com/watch?v=Sx1J3S6vUJ8), etc. 

We could also wing it, run the code, scroll through a few manual steps to check the buttons appear in the right spots, and move on. We could even ask someone to manually review any UI changes each day.

These approaches are not cheap or scalable in a modern, fast-moving CI environment. Thus were begotten UI automation testing tools. [Selenium](https://www.selenium.dev) is the most well-known of these. 

The simple idea is to find web controls in the DOM (e.g. by CSS selector) and automate mouse clicking, moving, text validation, etc. This simulates the manual interaction, and allows us to verify that our UI elements are in the right place, correctly validate input, and so on. Note: this is by no means a replacement for proper usability design; presumably this type of UX would be handled first, and decide on fonts, themes, overall metaphor, information architecture, and so on. See [SENG310](https://heat.csc.uvic.ca/coview/course/2021091/SENG310)! 

In [Assignment 5](../project/assignment5.md) one deliverable is to automate some of the acceptance testing with Selenium. While it is possible to integrate this into the Cucumber BDD approach as well, it adds a lot of moving pieces. 

## How To 
1. Install Selenium + [web drivers](https://www.selenium.dev/documentation/webdriver/getting_started/install_drivers/) in your config/build files. Selenium needs special libraries to puppet the browsers. Chrome is probably the safest bet here. Make sure the version of the driver matches your browser!
3. Figure out the pre/post/context conditions. Typically "pre" will be some initial web browser state (load a page, visit an endpoint). The "post" will reflect the page after some Context has been provided (e.g. a form input). 
4. Follow the code I've posted in the template repo. [Here is an invite](https://classroom.github.com/a/xYUOkaS8) to create your own repo. 
5. Let Selenium do the rest! It will open a browser, move the cursor, "click" buttons, etc.
6. [Read more on Selenium scripts.](https://www.selenium.dev/documentation/webdriver/getting_started/first_script/)

Note here we use async because we don't know how long the browser might take to do things (with a timeout cap). This can be tricky because while we wait, the browser state may change (and in subtle ways that look the same to the user). See [Waiting Strategies](https://www.selenium.dev/documentation/webdriver/waits/).

