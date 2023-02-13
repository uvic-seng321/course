# Learning Outcomes
By completing this assignment, you should demonstrate your ability to:
* Learn how to verify requirements through test driven development. Learn how to apply continuous integration.

# Submission
You should submit all documents before 11:59PM on the required date. All documents should have a title page which has on it the course number and name, the title of your project; the name of your group, a list of members indicating who was responsible for which parts, and the date. All submissions should be done via Brightspace. Only one submission is required per group. A single pdf file should be submitted and should named A4_groupnumber_groupname.pdf.

# PEER Evaluation
For all group assignments, you will receive a peer evaluation form from TeamMates. Individual marks may vary based on contribution level as percieved by your peers. Individuals who do not submit the peer evaluation forms for an assignment will lose marks for that assignment.

# Assignment Details
This is a group assignment. The group formation is the same as that in Assignment 2.

In Assignment 2, your team created a set of user stories documenting requirements for a software system. In this assignment, your team will begin to implement this product using TDD and CI techniques. 

The stories that should be implemented are the user stories with Must Have priority from A2. You only need to develop the back-end functionality (no user interface is required). If a must have user story and the associated acceptance criteria are written with a focus on the user interface, carefully think about the back-end functionality that will be required to fulfil that user need on user interface. 

The product must be developed with one of Javascript, Typescript, or Java, and be tested using xUnit. Mocking can be used as required using Mockito or suitable mocking framework. If your team wants to do something different (e.g. Scala) please check with the TA first.

## Requirement Details: 
You may find the acceptance criteria for your must have requirements are lacking some details when you go to write your test cases. You should follow up with your potential users or the customer to obtain additional details as required.

## Development procedures: 
Use the private project repo setup in A2. You can use your preferred automated build tool. The project README must have a build badge and a code coverage badge (see https://codecov.io) for the master branch. 

Your GitHub repository must show evidence that TDD and CI principles have been practiced. To do this, for each user story, create a new branch in your GitHub repository. On that branch, commit your small incremental changes. Each new test case should have two to four associated commits in this order:

1. Add failing test case
2. Add code to fix compile errors (if required) 
3. Add code to make test case pass
4. Refactor (as needed)

After the test case passes and the code/tests have been refactored as needed, the code should be merged into the master branch.

In addition to developing unit tests for each of the user stories, you should also create at least three integration tests to demonstrate that the different units work together. Clearly differentiate the unit and integration tests.

# Submission
You must submit a report that includes:
* A link to your private GitHub repository.
* All of your must have user stories and the associated acceptance criteria. Clearly show any changes that have been made to the user story or the acceptance criteria since A2.
* Organized by user story, for each acceptance criteria:

  * show the associated test cases (e.g. using screen shots or code snippets)
  * if mocking was used, explain why it was needed
  * if the acceptance criteria could not be tested, explain why (e.g. some may be related only to the UI)
* For each integration test:
   * show the test case (e.g. using screen shots or code snippets)
   * explain the interaction between the two units and why it should be tested
* A traceability matrix that maps each user story to the associated test cases
* A brief discussion on your team’s experience using CI and TDD to verify the user stories. 

Discuss why acceptance criteria needed to be changed (if applicable). Remember that user stories are a promise for a future conversation, so it is okay if you needed more details. The focus should be on what you learned about requirements by using TDD and CI. This discussion should be one to two pages.
 
# Marking Criteria
- All required information provided in sufficient detail
- The report is clear, well formatted, and professional
- Appropriate changes have been made to the user stories and acceptance criteria
- Test cases appropriate for acceptance criteria
- Appropriate integration tests
- Mocking used appropriately
- GitHub repository demonstrates TDD and CI principles and best practices have been
- applied
- Traceability matrix is accurate and well formatted
- Discussion clearly relates to software requirements and demonstrates appropriate
- understanding of the CI/TDD principles
- Peer evaluations

# Late Submissions
No late submissions. 
If you have a legitimate reason for submitting late, discuss this with the lecturer well in advance of the assignment due date.
