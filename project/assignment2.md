# Assignment Deadlines
1. 2 weeks before deadline: Project groups formed with group name and repo.
2. 11 days before deadline: Project ideas due on Brightspace and in lab. TAs will give feedback. 
4. 11-1 days prior: data gathering and follow-up meetings with potential users as needed
5. 0 days prior: all materials due on Brightspace.

# Project Description
This project is fairly open-ended. Your team will identify a business need, identify customers and stakeholders, and then gather requirements to begin solving that need.

The next 2 assignments for the group revolve entirely around the set of requirements you identify here, so choose a set that are a) implementable by April 9 b) in a domain you understand c) not obvious or repetitive.

# Learning Outcomes
By completing this assignment, you should demonstrate your ability to:

* elicit requirements from various sources, 
* perform requirements analysis and prioritization, 
* write requirement specifications, 
* validate and estimate requirements. 
* Focus on the problem, not solution.

# Submission
You should submit all documents before 11:59PM on the required date. All documents should have a title page which has on it the course number and name, the title of your project; the name of your group, a list of members indicating who was responsible for which parts, and the date. A single pdf file should be submitted and should named A2_groupname.pdf. All submissions should be done via Brightspace. Only one submission is required per group.

#  PEER Evaluation
For all group assignments, you will receive a peer evaluation form from TeamMates. Individual marks may vary based on contribution level as perceived by your peers. Individuals who do not submit the peer evaluation forms for an assignment will lose marks for that assignment.

# Assignment Details
## Step 0 Group formation: 
This is a group project. Each student must complete this project in a team of 3-4 students. Students should self-organise into teams. Each team should choose a group name (keep them classroom appropriate please). 

Once you have formed a team, you should self-enrol to one of the Project Groups on Brightspace's groups page. New groups should not be created. All students must be allocated to one of the lecturer-created groups. Groups must be formed and team names submitted by the deadline listed above. Students not assigned to groups by this time will be automatically assigned. 

Once your group is ready, accept the invitation to the Classroom assignment to instantiate a blank repo in the class Github repository. This will be your workspace. **All work should take place on GitHub including text edits**. Do not use Google Docs - upload Markdown docs. 

All team discussions should take place on Github (via the Discussions tab) or on Teams. This is important so the TAs can monitor your progress and help out when needed. 

## Step 1 Product vision and users:
You will choose a product or API with an active development team and engaged set of users. I have listed some in the appendix to this document. 

Identify your stated overall vision and scope for the improvements in a vision and scope document (text p81; 1 page-500 words). Define a simple context diagram (fig 5-6) showing the overall system context (e.g., external services/APIs used, authentication providers, etc.). 

Identify the customers and users of this tool using a stakeholder map like that in Table 6-1. 

## Step 2 Requirement extraction:
Requirements come from a variety of sources, including existing products, user feedback, crowd-sourced conversations, and interviews and surveys. Use some combination of these to derive a set of requirements for your product or additional features.

Use the NLP tools we examined to extract well known features from the crowd-RE data (e.g., Reddit threads). You should supplement this with some of the following:
- existing feature roadmaps (e.g. on GitHub)
- interviewing other users (such as your friends or existing users/devs) 
- extracting requirements from older products or similar products.

Your goal is to produce a set of at **least 10 user stories**. You will write user stories (on GitHub, using issues) through an iterative process. Your submission should include a draft version, with some high level ideas; a refined version 2, where you identify 10 user stories; and the final version, 3, which has been validated with existing users. A lot of the marks in this assignment are based on *where* the requirements came from and *how well* you justify their importance. Merely saying your team thinks they are useful is not sufficient.

Required documention includes:

### Project overview (1 page max). 
This should provide a brief description of the project, why it is needed and the overall goals of the software.
### Story map (1 page). 
This should be well laid out and easy to understand. Stories should be grouped into logical high-level activities and the activities should be displayed in chronological order. Highest priority stories should be at the top.
### Context, Vision, and Users
2-3 pages showing the project feature context, vision, and stakeholder maps.

### User story “cards”. 
For each user story on the story map, a user story **on GitHub** should be created with additional details for each user story. Each user story must have an ID Number, Title, User story statement (As a ... ), and priority. Stories should be prioritized using MoSCoW as discussed in class.
* The high priority (must have) stories should have acceptance criteria (checklist style). Acceptance criteria should be specific and detailed. After the initial version, you must have a follow-up process to get the additional details on the high priority stories to enable you to write detailed acceptance criteria. If you have follow-up questions for a “customer”, ask those early.
* The high priority stories must have estimates using story points (relative units). You can choose your preferred estimation technique. In an appendix, you must explain which estimation technique you selected, what scale is being used, and why you believe this is appropriate for your project.
* You may also use other requirement modeling techniques (e.g. flow charts, truth tables, low fidelity prototypes) for the high priority user stories (as required for complex user stories). Select the most appropriate technique.

### References: Any other documents that were used or consulted to develop the requirements should be referenced.

### Appendices:
1. Preparation. An appendix that includes all oftechniques your team used to find requirements. If you did interviews with friends or acquaintances, include the initial set of prepared interview questions , uploaded to the Brightspace assignment on the due date listed.
2. Elicitation evidence. All meetings, online repositories, and other forms of elicitation should be listed
(with the date, who participated, and any other relevant details).

# Marking Criteria
- All required information provided in sufficient detail
- The purpose of the system is explained correctly
- Story map clear, accurate, and well formatted
- Vision document is well written and easy to understand.
- Requirements are clear, complete, and consistent
- Rationale for requirements is well described
- Requirements have reasonable priorities
- Requirements have reasonable estimates
- Acceptance criteria well thought out, specific and detailed
- Evidence of thorough elicitation: follow-ups with potential users, document analysis, NLP techniques used, thoroughness of sources examined.
- Peer evaluations

# Late Submissions
No late submissions are allowed.

If you have a legitimate reason for submitting late, discuss this with the lecturer and your group well in advance of the assignment due date.

# Appendix: Potential Projects
A simple version of this project is to find an open feature request and expand on that. For example, [Node](https://github.com/nodejs/node/labels/feature%20request) has a bunch of open feature requests that conceivably count. Two problems: 1, these are likely beyond of your abilities to fix; 2, they are already pretty well specified, so there isn't a lot of RE to do. So you should find feature requests for a product that aren't well specified (yet). 

1. **Mastodon**: searching Mastodon's decentralized graph is non-trivial. A project could build a search function proof of concept, expanding on the specific user stories to build an MVP. See https://www.tbray.org/ongoing/When/202x/2022/12/30/Mastodon-Privacy-and-Search
3. Build some new feature on **existing APIs** like GitHub's or Stack Overflow. For example, maybe you have a "ChatGPT" detector that you could build using the API.
4. Existing clubs: your team could cozy up to the members of FormulaSAE, Robotics, CubeSat, GameDev, etc. Those students are a good source of ideas, would be excellent to interview, and  work on cool projects. Maybe you want to build a "FormulaSAEBot" for their Discord. 
5. Better Scientific Software: talk with your chemistry or sceince friends about a programming problem they have, e.g. with an open source library for analyzing CERN data. Mine CERN mailing lists for support.