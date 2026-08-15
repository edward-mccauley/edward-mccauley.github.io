# Enhancement Two Narrative: Algorithms and Data Structures

**Artifact:** Grazioso Salvare Dashboard  
**Category:** Algorithms and Data Structures  
**Student:** Edward McCauley  

## Artifact Description

The artifact I selected is the Grazioso Salvare Dashboard, a Python and MongoDB dashboard originally created earlier in my Computer Science program for advanced programming coursework. The dashboard was designed to display animal shelter data and support rescue-animal selection through filters and database interaction.

The original dashboard could filter animal records based on rescue categories, but the selection process was mostly based on direct filtering. It returned records that matched selected criteria, but it did not rank results or show which animals were the strongest candidates. This made the dashboard useful for narrowing records, but it left room to improve the decision-making process.

## Justification for Inclusion

I included this artifact in my ePortfolio because it gave me the opportunity to demonstrate algorithms and data structures in a practical application. Instead of only showing that data could be retrieved and filtered, I wanted to improve how the application evaluated animal records and supported rescue-animal selection.

For this enhancement, I added a rescue-animal matching and ranking system. Instead of only returning matching records, the enhanced version evaluates animals against rescue criteria, assigns scores, tracks matched traits, and ranks the strongest candidates first.

The enhanced version adds structured rescue profiles, scoring logic, and ranked results. The main improvements include:

- Rescue criteria stored in dictionaries for each rescue type
- Matching logic that compares animal records against rescue requirements
- A scoring system that assigns points based on breed, sex, and age matches
- A ranked output that sorts stronger rescue candidates ahead of weaker matches
- Sample animal records that allow the algorithm to be reviewed without requiring a live database connection

The main files related to this enhancement include:

- `rescue_filter_service.py`: contains rescue profiles, matching logic, scoring, and ranking
- `sample_animals.py`: provides sample animal records for review mode
- `dashboard_controller.py`: coordinates the rescue matching process
- `app.py`: demonstrates ranked sample results for review

This enhancement showcases my ability to apply algorithmic thinking to a real application. I used dictionaries to organize rescue criteria, lists to process animal records, conditional logic to evaluate matches, and sorting to rank results by score. The enhancement also improves maintainability because the rescue criteria are easier to review and update. If a rescue category changes in the future, the criteria can be adjusted in one location instead of being scattered throughout the dashboard code.

## Reflection on the Enhancement Process

During this enhancement, I learned how algorithms and data structures can improve the usefulness of an application. The original dashboard could filter animal records, but the enhanced version provides more meaningful decision support by scoring and ranking candidates. This helped me see that algorithms are not only about solving abstract problems. They can directly improve how users interpret data and make decisions.

One challenge I faced was keeping the matching logic understandable while still making it more useful than a basic filter. I did not want the scoring system to become overly complicated or difficult to explain. I addressed this by organizing rescue criteria in dictionaries and using clear scoring rules that can be reviewed, tested, and adjusted.

Another challenge was demonstrating the enhancement without depending on a live MongoDB connection. I addressed this by adding sample animal records and review-mode output so the matching and ranking logic could be reviewed independently. This made the enhancement easier to test and easier for an instructor or future reviewer to understand.

The feedback and direction from earlier milestones helped me keep the enhancement focused. Since Enhancement One improved the project structure, I was able to place the algorithm logic into a separate service instead of adding more logic directly into the dashboard. This made the algorithm enhancement cleaner and easier to connect to the overall application design.

This enhancement improved the artifact by changing the rescue-animal selection process from simple filtering into a more structured matching and ranking system. The enhanced version is more useful because it not only identifies possible candidates but also helps prioritize stronger matches.

## Course Outcome Alignment

This enhancement supports the following CS 499 course outcomes:

- **Course Outcome 1:** Supports decision-making by improving how rescue-animal candidates are evaluated and ranked.
- **Course Outcome 2:** Demonstrates professional communication through clear code organization, comments, documentation, and this enhancement narrative.
- **Course Outcome 3:** Demonstrates the use of algorithms and data structures to solve a practical computing problem.
- **Course Outcome 4:** Supports software engineering practices by organizing the matching logic into a separate service module.
- **Course Outcome 5:** Supports a security and quality mindset by keeping the matching logic controlled, readable, and easier to validate.

This enhancement most strongly supports Course Outcome 3 because it demonstrates the use of data structures, conditional logic, scoring, and sorting to solve a practical problem. It also partially supports the communication, software engineering, and security outcomes because the algorithm is documented, separated into its own service, and easier to validate. The database outcome is not the primary focus of this enhancement and is demonstrated more directly in Enhancement Three.

## GitHub Repository

The code for this enhancement is available here:

[View Enhancement Two Code Repository](https://github.com/edward-mccauley/CS499-Grazioso-Salvare-ePortfolio)

## Downloadable Narrative

[Download Enhancement Two Narrative](documents/enhancement-two-narrative.docx)

## Return to Home

[Return to ePortfolio Home](https://edward-mccauley.github.io)
