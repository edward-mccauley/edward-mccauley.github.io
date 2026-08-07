# Enhancement Two: Algorithms and Data Structures

**Artifact:** CS-340 Grazioso Salvare Dashboard  
**Category:** Algorithms and Data Structures  
**Student:** Edward McCauley  

## Enhancement Overview

For Enhancement Two, I improved the algorithms and data structures portion of my CS-340 Grazioso Salvare Dashboard artifact. The original project used Python and MongoDB to display animal shelter data and support rescue-animal selection through dashboard filters.

The original dashboard could filter animal records based on rescue categories, but the selection process was mostly based on direct filtering. For this enhancement, I improved the logic by adding a rescue-animal matching and ranking system. Instead of only returning matching records, the enhanced version evaluates animals against rescue criteria, assigns scores, tracks matched traits, and ranks the strongest candidates first.

This enhancement demonstrates my ability to use algorithms and data structures to solve a practical problem and make the application more useful for decision-making.

## What Was Improved

The enhanced version adds structured rescue profiles, scoring logic, and ranked results. The main improvements include:

- Rescue criteria stored in dictionaries for each rescue type
- Matching logic that compares animal records against rescue requirements
- A scoring system that assigns points based on breed, sex, and age matches
- A ranked output that sorts stronger rescue candidates ahead of weaker matches
- Sample animal records that allow the algorithm to be reviewed without requiring a live database connection

The original version focused mainly on filtering data. The enhanced version improves the decision-making process by ranking animals according to how well they match the rescue profile.

## Files Involved

The main files related to this enhancement include:

- `rescue_filter_service.py`: contains rescue profiles, matching logic, scoring, and ranking
- `sample_animals.py`: provides sample animal records for review mode
- `dashboard_controller.py`: coordinates the rescue matching process
- `app.py`: demonstrates ranked sample results for review

## Skills Demonstrated

This enhancement showcases my ability to apply algorithmic thinking to a real application. I used dictionaries to organize rescue criteria, lists to process animal records, conditional logic to evaluate matches, and sorting to rank results by score.

The enhancement also improves maintainability because the rescue criteria are easier to review and update. If a rescue category changes in the future, the criteria can be adjusted in one location instead of being scattered throughout the dashboard code.

## Course Outcome Alignment

This enhancement supports the following CS 499 course outcomes:

- **Course Outcome 1:** Supports decision-making by improving how rescue-animal candidates are evaluated and ranked.
- **Course Outcome 2:** Demonstrates professional communication through clear code organization, comments, documentation, and this enhancement writeup.
- **Course Outcome 3:** Demonstrates the use of algorithms and data structures to solve a practical computing problem.
- **Course Outcome 4:** Supports software engineering practices by organizing the matching logic into a separate service module.
- **Course Outcome 5:** Supports a security and quality mindset by keeping the matching logic controlled, readable, and easier to validate.

## GitHub Repository

The code for this enhancement is available here:

[View Enhancement Two Code Repository](https://github.com/edward-mccauley/CS499-Grazioso-Salvare-ePortfolio)

## Return to Home

[Return to ePortfolio Home](https://edward-mccauley.github.io)
