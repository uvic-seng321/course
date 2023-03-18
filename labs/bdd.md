# Using Cucumber

## What To Do in Lab
1. Read through the material below. 
2. Copy the repo using the invite. 
3. Complete the tests so that Cucumber reports a passing test.
4. Design your BDD test plans for assignment 5. You should have a completed test plan that maps user stories (features) to a set of feature specs and corresponding code. 
5. Your group should be able to write all the Gherkin language (the `.feature` files) in lab. That would leave someone to implement the steps and wire the tests into the system. 

## Overview
This lab follows the excellent resources at https://school.cucumber.io/courses/take/bdd-with-cucumber-javascript/ Feel free to follow those as well.

   1. [Accept the invite](https://classroom.github.com/a/PGQCFij_) to create a template with a codespace and Node/Cucumber preinstalled.
   2. Open Codespaces or clone it locally. 
   3. Run `npm test` to see the Cucumber report.

What is going on here? Cucumber has several key ideas. One is that we define our **features** (aka requirements) in a file (written in Gherkin language). `hear_shout.feature` is a feature of our sample app. Each feature has several scenarios (happy path, error path etc). 

For each scenario we define preconditions (`given`), context (`when`), and postconditions (`then`). These correspond to acceptance criteria for our user stories (in this case, that "receiver hears the message")

The feature file is a way of writing down the requirements. But how do we link this to our code? After all, this is a testing approach. 

Much like in TDD, with BDD we will first define the "behavior" the system needs to exhibit ("the code we wish we had"). We then write code to make that true. Note that in each of Given/When/Then we are writing code: to set up the preconditions, to check the context, and finally (most importantly) we are checking the output matches the acceptance test criteria.

In Cucumber we need to wire our feature to the steps it should be following (`steps.js`). In that file, the stuff in {} represents the parameterized calls to the actual source code we will write. It is pretty simple to wire things in - we are just pattern-matching on the features. 

In the repo you created, find these files and ensure you see how they are connected.

Now, let's do a bit of coding to make this simple feature work. Your error message when doing `npm test` should reflect that we haven't **designed** the implementation to make this feature work. Much like unit testing, we want to first specify the *behavior*, then *implement* the spec to make this work. 

And just like in unit testing, we will need to **refactor** the code as we go and learn more about the best design. E.g., maybe `Person` is not the place to handle movement. 

# Next steps
We aren't done with this feature - we need to make the final "Then" step pass. First, add the assertion library in `steps.js` after line 2:

`const { assertThat, is } = require('hamjest')`

Now you can use [hamjest's `assertThat()`](https://www.npmjs.com/package/hamjest) method to do assertion checks. 

Insert a check in the `Then` section of the `steps.js` to implement the appropriate test. Again, write the code you think should be there (something like `Person.messagesHeard()`). Then go to `shouty.js` and make the test pass (i.e., write the business logic).

Hint: you will need to persist the message the "sean" object shouted into the Then portion of the code.

Feel free to solve this in the dumbest way possible. We can always add a new scenario, with a different message, to see if our code can handle it. One key idea in TDD/BDD is to do the minimal amount necessary in each step, in order to stay DRY (don't repeat yourself). 