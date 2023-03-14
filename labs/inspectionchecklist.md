# Inspection Checklists

## Requirements (after Wiegers)
1. Do requirements exhibit a clear distinction between functions and data?
2. Do requirements define all the information to be displayed to users?
3. Do requirements address system and user response to error conditions?
4. Is each requirement stated clearly, concisely, and unambiguously?
5. Is each requirement testable?
6. Are there ambiguous or implied requirements?
7. Are there conflicting requirements?
8. Are there areas not addressed in the requirements that need to be?
12. Are there requirements that contain an unnecessary level of design detail?

### Items that may or may not apply to our project
9.  Are performance requirements (such as response time, data storage requirements) stated?
10. If the requirements involve complex decision chains, are they expressed in a form that facilitates comprehension (i.e., decision tables, decision trees, etc.)?
11. Have requirements for performing software upgrades been specified?
13. Have the real-time constraints been specified in sufficient detail?
14. Has the precision and accuracy of calculations been specified?
15. Is it possible to develop a thorough set of tests based on the information contained in the SRS? If not, what information is missing?
16. Have Assumptions and Dependencies been clearly stated?
17. Does the document contain all the information called out in the outline for the SRS?

## Design Checklists
Ideally, begin by identifying the key quality attribute scenarios. It is hard to come up with obvious design review questions without understanding the system context. Still, given the type of project we tackle in the course, you should review the following about the design:
1. Error-handling: does the design explain how errors are managed, and recovered from? 
2. Logging: is there a way to understand what is happening in the system (e.g., logins, pages requested, errors)
3. Data storage: is the design specific about what data is stored and where? 
4. Security: does the design explain a security model, including data-at-rest and data-in-transit? 
5. User management: how are user accounts managed? What is the authentication and identification approach?
6. Performance: how does the design accommodate performance demands, including out-of-sample (>2 standard dev.) spikes?
7. External components: does the design outline the components it relies on, and why? What is the update/versioning approach?
8. Call-graph: can the design explain how the system works in the happy path? 
9. Usability and UX: is there a front-end concept that presents a usable and coherent experience for the user? Are users identified?
10. Accessibility and internationalization (i18n): are there ways to accommodate accessibility requirements (alt. text) and the need to handle non-ASCII/English users?
11. Testing/devops: does the design make clear how the product is built and deployed? How does this work? Where is it running?

(feel free to add more - a good source is when you get confused about what is happening in your colleague's code!)

# Other readings
- [Google/Hillary design reviews](https://medium.com/git-out-the-vote/strengthening-products-and-teams-with-technical-design-reviews-ae6a1bec5216)
- [Design Doc template](https://docs.google.com/document/d/1uMHzRsEDZb_p9xfFGerCVhr-0mAi-d-OFY4jJi0dYk4/edit)
- [Test automation review](https://msdn.microsoft.com/en-us/library/ff521647.aspx)
- [Active Reviews for Intermediate Designs (ARID)](https://resources.sei.cmu.edu/asset_files/TechnicalNote/2000_004_001_13685.pdf)