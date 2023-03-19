# Learning Outcomes
By completing this assignment, you should demonstrate your ability to:
* apply behavior-driven development (BDD) principles and practices
* focus on features that deliver business value 
* define software behavior collaboratively
* illustrate features with concrete examples
* write executable specification
* deliver living documentation
* practice behavior-driven development (BDD) using Cucumber
* automate acceptance criteria for the UI using Selenium or similar tools


# Submission
You should submit all documents before 11:59PM on the required date. All documents should have a title page which has on it the course number and name, the title of your project; the name of your group, a list of members indicating who was responsible for which parts, and the date. All submissions should be done via Canvas. Only one submission is required per group. A single pdf file should be submitted and named as A5_groupnumber_groupname.pdf.

# PEER Evaluation
For all group assignments, you will receive a peer evaluation form from TEAMMATES. Individual marks may vary based on contribution level as perceived by your peers. Individuals who do not submit the peer evaluation forms for an assignment will lose marks for the assignment.

# Assignment Details
This is a group assignment. The group formation is the same as that in Assignment 2.

In Assignment 2, your team created a set of user stories documenting requirements for a software system. In this assignment, your team will implement this product using BDD practices and Cucumber. You need to implement the front-end part of the user stories you implemented in A4 and back-end can be reused or modified from A4 to work in a web application. In addition, you need to automate the UI of these user stories using an automation tool. The product must be developed with your language of choice, and a BDD tool such as Cucumber and demonstrate UI testing using automation tools such as Selenium Web driver.

## Copilot/ChatGPT
You are required to enable and use AI support tools in this assignment. BUT, you need to explain how they helped. Your job is to see if the AI is applying a concept properly. It might help to think of yourself as a marker, inspecting the submission ChatGPT makes. Your team will write a report summarizing your team's experiences.
1. Develop at least one feature/user story using **only** ChatGPT or Bing (GPT3.5/4). You can either use the web interface or a tool like [Rubberduck](https://marketplace.visualstudio.com/items?itemName=Rubberduck.rubberduck-vscode). You will need an OpenAI account. If your team has trouble with this step, you can use Copilot (GPT3) as a workaround. Copilot seems to be less helpful, so your results will be more useful with the other tools.
2. An important and emerging skill, not unconnected to RE, is *prompt engineering*, i.e., tailoring the output of the AI. 
3. Prompt ChatGPT three times. The first session should be pretty basic - try giving it the spec as a javascript comment. In Prompt 2, add more refinements (e.g., domain knowledge). In the third prompt, **co-editing**, give the AI specific feedback ("the function in line 20 should take an Int"). 
   1. Record each of the prompts you used and the tool's suggestion.  
4. Each time the AI suggests something wrong or unhelpful, make a note. 
5. Prepare a report, around 1000 words, that outlines:
   1. the prompts you used, and the feature involved;
   2. your group's reflection on where ChatGPT struggled, and why;
   3. your group's wider reflection on how useful the tool was, compared with DIY coding.
      1. what potential bias or accuracy problems might exist?
      2. how does it replace or augment skills you've learned in undergrad?
      3. what role would RE play if these tools were widespread?

## Requirement Details: 
You may find the acceptance criteria for your must have requirements are lacking some details when you go to write your test scenarios following Gherkin format. You should follow up with your potential users or the customer to obtain additional details as required.

## Development procedures: 
Your GitHub repository must show evidence that BDD principles have been practiced. To do this, for at least three features/stories, create a new branch in your GitHub repository. On that branch, commit your small incremental changes.
* Each scenario should have associated commits in this order against a feature:
  * Write a failing scenario
  * Implement step definitions
  * Write the automation and application code
  * Refactor (as needed)
* Demonstrate appropriate use of Cucumber options such as hooks, tags etc., and features
such as implementing scenario outlines, data tables, backgrounds etc.
* Automation of the UI part of the user stories
* Identifying and interacting with web elements

## Submission:
You must submit a report that includes:
* A link to your private GitHub repository created for A5.
* All the must have user stories under features. Clearly show any changes that have been
made to the feature set or the acceptance criteria since A2 and A4.
* Organized by features, for each scenario
  * show the associated steps (e.g. using screen shots or code snippets)
* A detailed report generated using any 3rd party Cucumber reporter plugins in a
professional format
* Read Me to guide the markers on how to run the application.
* Design reflection from the lab of Mar 14.
* ChatGPT reflection from above.

# Marking Criteria
* Demonstration of applying BDD principles and best practices during the development.
* All the required application features have been reasonably implemented and automated.  
* The quality of the source code.
* The content, organization and presentation of the report.
* Taking peer evaluation into consideration.

# Late Submissions
No late submissions.
If you have a legitimate reason for submitting late, discuss this with the lecturer well in advance of the assignment due date.
