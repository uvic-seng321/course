**This is an individual assignment. All students are required to work independently.**

# Instructions
You are required to perform the following tasks:
1. Follow this invite link to create your own individual GitHub repo. Setup GitHub Actions in the repository (see the Setting up GitHub Actions instructions in the lab slides if you are unfamiliar with this).
2. Add a [continuous integration build badge](https://docs.github.com/en/actions/monitoring-and-troubleshooting-workflows/adding-a-workflow-status-badge) to your README.
3. The repo should already contain the following files:
    1. Calculator.ts: a class that adds and multiplies sets of  Integers
    2. StringCheck.ts: a class that checks if a string is a palindrome, is empty, is null, or contains only whitespace.
    3. CalculatorTest.spec.ts: a test class to ensure that the Calculator class is working as intended.
    4. StringCheckTest.spec.ts: a test class to ensure that the StringCheck class is working as intended.
**Note**: You will be required to write some code to ensure that the classes are working as intended and are tested appropriately (there are comments in the files explaining this). These changes should be done as part of step 4* ensure you first do step 4 and upload the original code to your repository.
1. Create a Java project using the code in step 3 and create a build file using Gradle, Maven, or Ant. Upload the java project to the GitHub repo you created in step 1. Actions should show the build is failing. 
2. Create a new branch in your repository. Write the missing test cases, fix the broken test cases, and write the additional code as described in the comments in each file.
3. Once all tests are passing, submit a Pull Request from your newly created branch to the master branch with these code changes. Do not merge the Pull Request. GitHub Actions should 
show that the pull request passes all checks.

# Learning Outcomes
By completing this assignment, you should demonstrate your ability to set up a continuous integration environment and write a simple test suite.

# Submission
You should submit a link to your private repository before 11:59PM on the required date through the Brightspace assignment. The teaching assistants will submit additional pull requests to your repository after the assignment deadline to ensure the code works as expected and that continuous integration is setup appropriately.

# Marking Criteria
* Private GitHub repository created with actions enabled
* Provided code has been fixed and completed in a new branch
* A pull request with the required code changes has been submitted
* The build shows the submitted pull request is passing all checks
* The GitHub README file includes the build status badge
* The badge on the README and the other build indicators change status
appropriately when additional pull requests are submitted by the teaching team

# Late Submissions
No late submissions. If you have a legitimate reason for submitting late, discuss this with the lecturer well in advance of the assignment due date.