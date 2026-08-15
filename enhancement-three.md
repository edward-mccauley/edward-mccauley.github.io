# Enhancement Three Narrative: Databases

**Artifact:** Grazioso Salvare Dashboard  
**Category:** Databases  
**Student:** Edward McCauley  

## Artifact Description

The artifact I selected is the Grazioso Salvare Dashboard, a Python and MongoDB dashboard originally created earlier in my Computer Science program for advanced programming coursework. The dashboard was designed to display animal shelter data and support rescue-animal selection through filters and database interaction.

The original artifact connected directly to MongoDB and used database queries to retrieve animal records. While the original version functioned for the course project, the database access logic could be improved to make the application safer, more maintainable, and easier to review. The original version handled database logic more directly inside the database access class, which left room to improve validation, configuration, error handling, and control over query behavior.

## Justification for Inclusion

I included this artifact in my ePortfolio because it gave me the opportunity to demonstrate database skills in a practical software application. The dashboard depended on MongoDB to retrieve and manage animal shelter records, so improving the database layer was an important part of making the overall artifact more professional.

For this enhancement, I added a more controlled database query layer that validates fields, limits accepted operators, applies projections, controls result limits, and improves database error handling. These changes improved how the application communicates with MongoDB and made the database layer safer and easier to maintain.

The enhanced version improves the MongoDB database layer by adding safer query construction and validation. The main improvements include:

- A dedicated `database_query_service.py` module
- Allowed filter fields for database queries
- Allowed update fields for database updates
- Allowed MongoDB operators such as `$eq`, `$in`, `$gte`, and `$lte`
- Projection support to control which fields are returned
- Result limit validation to prevent overly large queries
- Safer update handling
- Improved error handling for database operations
- Environment-based configuration support through `config.py`
- A `.env.example` file to document expected configuration without exposing real credentials

The main files related to this enhancement include:

- `database_query_service.py`: validates query fields, operators, projections, updates, and limits
- `animal_shelter.py`: uses the query service to perform safer MongoDB operations
- `config.py`: stores database configuration using environment variable support
- `dashboard_controller.py`: coordinates application requests with the database layer
- `app.py`: demonstrates database review mode output
- `.env.example`: documents expected environment variable configuration without exposing real credentials

This enhancement showcases database design, validation, configuration management, and security skills. I improved the artifact by separating query validation from direct database communication, controlling which fields and operators can be used, limiting query results, and removing hard-coded credentials from the enhanced source code.

## Reflection on the Enhancement Process

During this enhancement, I learned that database access should be designed carefully because it affects reliability, maintainability, and security. A database layer should not only retrieve data. It should also control how queries are built, what fields are allowed, how much data can be returned, and how errors are handled.

One challenge I faced was improving the database layer without making the project too complex. I wanted the enhancement to be meaningful, but I also wanted the code to remain understandable for review. I addressed this by creating a separate `DatabaseQueryService` that handles validation while allowing the `AnimalShelter` class to remain focused on MongoDB communication.

Another challenge was demonstrating the database enhancement without requiring a live MongoDB connection for every reviewer. I addressed this by adding database review-mode output in `app.py`, which shows safe query construction, projection handling, and result limit validation. This made the enhancement easier to review and helped show the database improvements even when the database is not running locally.

I also incorporated final-submission guidance by cleaning up configuration and repository content. Since the ePortfolio and artifact repository are public-facing, I removed hard-coded credentials from the enhanced source code and added an `.env.example` file to show how environment variables should be configured. This supports a more professional and security-aware project presentation.

This enhancement improved the artifact by making database operations more controlled, safer, and easier to review. The enhanced version separates query validation and database communication into clearer responsibilities, reduces the risk of unrestricted database operations, and better supports maintainability.

## Course Outcome Alignment

This enhancement supports the following CS 499 course outcomes:

- **Course Outcome 1:** Supports decision-making by improving how database records are retrieved, controlled, and prepared for application use.
- **Course Outcome 2:** Demonstrates professional communication through clear documentation, code organization, configuration notes, and this enhancement narrative.
- **Course Outcome 3:** Supports thoughtful design choices involving query construction, validation, limits, and tradeoffs.
- **Course Outcome 4:** Demonstrates the use of computing tools and techniques by improving the MongoDB access layer and separating database responsibilities.
- **Course Outcome 5:** Supports a security mindset through safer query validation, environment-based configuration, result limits, projections, and controlled database error handling.

This enhancement most strongly supports Course Outcome 5 because it focuses on safer database access, validation, configuration handling, and controlled error handling. It also strongly supports Course Outcome 4 because it improves how the application uses MongoDB and separates database responsibilities into a cleaner structure. Course Outcome 3 is partially supported through query validation, limits, and design tradeoffs, but the primary algorithms and data structures work is demonstrated more directly in Enhancement Two.

## GitHub Repository

The code for this enhancement is available here:

[View Enhancement Three Code Repository](https://github.com/edward-mccauley/CS499-Grazioso-Salvare-ePortfolio)

## Downloadable Narrative

[Download Enhancement Three Narrative](documents/enhancement-three-narrative.docx)

## Return to Home

[Return to ePortfolio Home](https://edward-mccauley.github.io)
