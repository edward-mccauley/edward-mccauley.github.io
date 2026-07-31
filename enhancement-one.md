# Enhancement One: Software Design and Engineering

**Artifact:** CS-340 Grazioso Salvare Dashboard  
**Category:** Software Design and Engineering  
**Student:** Edward McCauley  

## Enhancement Overview

For Enhancement One, I improved the software design and engineering structure of my CS-340 Grazioso Salvare Dashboard artifact. The original project was created in CS-340: Advanced Programming Concepts and used Python and MongoDB to display animal shelter data and support rescue-animal selection through a dashboard application.

The original artifact functioned as intended for the course project, but several responsibilities were closely connected within the dashboard notebook. The notebook handled layout, filtering behavior, user interaction, display updates, and database calls. For this enhancement, I refactored the project into a more organized, layered structure so that each major part of the application has a clearer responsibility.

This enhancement demonstrates my ability to take a working academic project and improve its internal design so that it is easier to understand, maintain, test, and extend.

## What Was Improved

The enhanced version separates the project into multiple components:

- `app.py`: application entry point
- `animal_shelter.py`: MongoDB database access layer
- `config.py`: configuration values and environment variable support
- `rescue_filter_service.py`: rescue criteria and filter-building logic
- `dashboard_controller.py`: coordination layer between the dashboard, filters, and database
- `README.md`: documentation describing the enhancement and review mode

The original version grouped several responsibilities together. The enhanced version applies separation of concerns by giving each file a more specific purpose. This makes the project easier to review and provides a stronger foundation for later enhancements in algorithms, data structures, and databases.

## Skills Demonstrated

This enhancement showcases software engineering skills such as modular design, class-based organization, configuration management, documentation, and maintainability. The updated structure makes the project easier for another developer, instructor, or stakeholder to understand because the major responsibilities are separated into clearer components.

The enhancement also supports a stronger security mindset. Database configuration is no longer buried directly inside the database access class, and the enhanced version supports environment variables for configuration values. Error handling was also improved so that database errors can be handled more safely and consistently.

## Course Outcome Alignment

This enhancement supports the following CS 499 course outcomes:

- **Course Outcome 1:** Supports collaboration and decision-making through clearer organization, documentation, and maintainable structure.
- **Course Outcome 2:** Demonstrates professional communication through README documentation, code comments, the code review, and the enhancement narrative.
- **Course Outcome 4:** Demonstrates software engineering practices such as modular design, separation of concerns, class-based organization, and iterative improvement.
- **Course Outcome 5:** Supports a security mindset through improved configuration handling and safer error handling.

## GitHub Repository

The code for this enhancement is available here:

[View Enhancement One Code Repository](https://github.com/edward-mccauley/CS499-Grazioso-Salvare-ePortfolio)

## Return to Home

[Return to ePortfolio Home](https://edward-mccauley.github.io)