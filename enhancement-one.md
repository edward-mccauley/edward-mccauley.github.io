# Enhancement One: Software Design and Engineering

**Artifact:** CS-340 Grazioso Salvare Dashboard  
**Category:** Software Design and Engineering  
**Student:** Edward McCauley  

## Enhancement Overview

For Enhancement One, I improved the software design and engineering structure of my CS-340 Grazioso Salvare Dashboard artifact. The original project was created in CS-340: Advanced Programming Concepts and used Python and MongoDB to display animal shelter data and support rescue-animal selection through a dashboard application.

The original artifact worked for the course project, but several responsibilities were closely connected. The dashboard notebook handled layout, filtering behavior, user interaction, display updates, and database calls. For this enhancement, I refactored the project into a more organized, layered structure so that each major part of the application has a clearer responsibility.

## What Was Improved

The enhanced version separates the project into multiple components:

- `app.py`: application entry point
- `animal_shelter.py`: MongoDB database access layer
- `config.py`: configuration values and environment variable support
- `rescue_filter_service.py`: rescue criteria and filter-building logic
- `dashboard_controller.py`: coordination layer between the dashboard, filters, and database
- `README.md`: documentation describing the enhancement and review mode

This enhancement demonstrates software engineering skills such as modular design, separation of concerns, class-based organization, configuration management, documentation, and maintainability.

## Skills Demonstrated

This enhancement showcases my ability to take an existing academic project and improve it into a more professional software artifact. The updated structure makes the project easier to understand, maintain, test, and extend. It also supports a stronger security mindset by reducing hard-coded configuration inside the database class and improving how errors are handled.

## Course Outcome Alignment

This enhancement supports the following CS 499 course outcomes:

- **Course Outcome 1:** Supports collaboration and decision-making through clearer organization and documentation.
- **Course Outcome 2:** Demonstrates professional communication through README documentation, code comments, and the enhancement narrative.
- **Course Outcome 4:** Demonstrates software engineering practices such as modular design, separation of concerns, and iterative improvement.
- **Course Outcome 5:** Supports a security mindset through better configuration handling and safer error handling.

## GitHub Repository

The code for this enhancement is available here:

[View Enhancement One Code Repository](https://github.com/edward-mccauley/CS499-Grazioso-Salvare-ePortfolio)

## Return to Home

[Return to ePortfolio Home](README.md)