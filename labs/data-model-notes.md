# Data Modeling for Project

(see [the course slides](https://github.com/uvic-seng321/course/blob/main/modules/analyze/Data%20and%20process%20modeling%20--%20Structured%20Analysis.pdf) for details)

[Part of the deliverables](https://github.com/uvic-seng321/course/blob/main/project/assignment4.md#submission-1) for Assignment 4 are to demonstrate your team have thought about the 'backend' of the application your team is building.

What is a 'backend'? 
    - the part the users don't see
    - the part responsible for the Model and (possibly) Controllers in the MVC Pattern
    - the part where the data lives and is stored
    - jobs with titles like "DBA", "data engineer", "database analyst"
    - the important bits

Your submission should contain a sketch (or sketches) showing how the backend is built. The sketch should be accompanied by a data dictionary listing the specifics for each entity (e.g., "Customer has fields 'name', 'address'"). The data dictionary doesn't have to be very formal but should explain what each entity is doing in your system. 

The sketch should outline the external entities involved, the data flows for the key user stories (the Must-Haves), and then (very briefly) sketch out a software design for making this possible, naming the technologies you plan to use (e.g., Firebase, SQLite, native data stores .... you should not be storing data in memory only - your app must have persistence.)

## How to Start
There are two suggested approaches. One is to focus on the "things" in the domain and build up an ER diagram, showing how different entities (such as Game, Items, Players) are related. 
1. Begin naming these things, 
2. Sketch a box for each
3. Then think about how they connect.
4. Connect the entities with relationships (e.g., Player is many-to-many with Game, and the relationship is `plays`.). 

The problem with that approach is the end result is a static module view of the system that does not connect well to what will happen at run-time, i.e., what processes create these entities or use these entities?

Thus another, complementary approach is what we tried in class, with Data Flow Diagrams. These show how processes interact with data, and for some people is a more natural way to think about what is happening when the system runs (the components and connectors). 
1. Begin with your activities / use cases identified in Assignment 2. 
2. Pick an activity that covers most of the user stories you identified.
3. Explain the external data sources you do not control (e.g., Facebook credentials). 
4. Identify the processes that manipulate that data, thinking a bit ahead to how your team will implement that code.
5. Where is the data stored after the various processes are done with it? What reads that data? 