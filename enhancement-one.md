# Enhancement One Narrative: Software Design and Engineering

**Artifact:** Grazioso Salvare Dashboard  
**Category:** Software Design and Engineering  
**Student:** Edward McCauley  

## Artifact Description

 The artifact I selected is the Grazioso Salvare Dashboard, a Python and MongoDB dashboard originally created earlier in my Computer Science program for advanced programming coursework. The dashboard was designed to display animal shelter data and support rescue-animal selection through filters and database interaction.

The original artifact functioned as intended for the course project, but several responsibilities were closely connected within the dashboard notebook. The notebook handled layout, filtering behavior, user interaction, display updates, and database calls. This made the project work, but it also made the internal structure harder to maintain, test, and extend.

## Justification for Inclusion

I included this artifact in my ePortfolio because it gave me the opportunity to demonstrate software design and engineering skills using an existing working application. Instead of creating a new project from the beginning, I improved the structure of an existing artifact and made it more professional.

For this enhancement, I refactored the project into a more organized, layered structure so that each major part of the application has a clearer responsibility. The enhanced version separates the project into multiple components:

- `app.py`: application entry point
- `animal_shelter.py`: MongoDB database access layer
- `config.py`: configuration values and environment variable support
- `rescue_filter_service.py`: rescue criteria and filter-building logic
- `dashboard_controller.py`: coordination layer between the dashboard, filters, and database
- `README.md`: documentation describing the enhancement and review mode

This enhancement showcases my ability to apply modular design, separation of concerns, class-based organization, configuration management, documentation, and maintainability. The original version grouped several responsibilities together. The enhanced version gives each file a more specific purpose, which makes the project easier to review and provides a stronger foundation for later enhancements in algorithms, data structures, and databases.

The enhancement also supports a stronger security mindset. Database configuration is no longer buried directly inside the database access class, and the enhanced version supports environment variables for configuration values. Error handling was also improved so that database errors can be handled more safely and consistently.

## Reflection on the Enhancement Process

During this enhancement, I learned that improving software design is not only about making code look cleaner. It is about making the system easier to understand, maintain, test, and extend. A working project can still need improvement if its responsibilities are too closely connected or if future changes would be difficult to make.

One challenge I faced was deciding how much to refactor without turning the enhancement into a completely different project. I wanted to preserve the purpose of the original dashboard while improving the design in a meaningful way. I addressed this by keeping the original dashboard concept intact and focusing on the internal structure of the application.

I also incorporated instructor feedback that simple organization and cleanup would not be substantial enough by focusing on a more meaningful layered design. This feedback helped me move beyond basic file cleanup and focus on clearer responsibilities between the application entry point, controller logic, filtering service, database access layer, and configuration file.

This enhancement improved the artifact by transforming it from a tightly connected dashboard project into a more professional structure with clearer responsibilities. It also prepared the artifact for the later algorithm and database enhancements because the project was easier to extend once the major responsibilities were separated.

## Course Outcome Alignment

This enhancement supports the following CS 499 course outcomes:

- **Course Outcome 1:** Supports collaboration and decision-making through clearer organization, documentation, and maintainable structure.
- **Course Outcome 2:** Demonstrates professional communication through README documentation, code comments, the code review, and the enhancement narrative.
- **Course Outcome 4:** Demonstrates software engineering practices such as modular design, separation of concerns, class-based organization, and iterative improvement.
- **Course Outcome 5:** Supports a security mindset through improved configuration handling and safer error handling.

This enhancement most strongly supports Course Outcome 4 because it demonstrates the use of software engineering techniques, modular design, and iterative improvement. It also partially supports the communication, collaboration, and security outcomes because the improved structure, documentation, and configuration handling make the artifact easier to review, explain, and maintain. Course Outcome 3, which focuses on algorithms and data structures, is not the primary focus of this enhancement and is demonstrated more directly in Enhancement Two.

## GitHub Repository

The code for this enhancement is available here:

[View Enhancement One Code Repository](https://github.com/edward-mccauley/CS499-Grazioso-Salvare-ePortfolio)

## Downloadable Narrative

[Download Enhancement One Narrative](documents/enhancement-one-narrative.docx)

## Return to Home

[Return to ePortfolio Home](https://edward-mccauley.github.io)