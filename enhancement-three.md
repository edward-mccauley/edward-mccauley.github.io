# Enhancement Three: Databases

**Artifact:** CS-340 Grazioso Salvare Dashboard  
**Category:** Databases  
**Student:** Edward McCauley  

## Enhancement Overview

For Enhancement Three, I improved the database portion of my CS-340 Grazioso Salvare Dashboard artifact. The original project used Python and MongoDB to display animal shelter data and support rescue-animal selection through a dashboard application.

The original artifact connected directly to MongoDB and used database queries to retrieve animal records. While the original version worked for the course project, the database access logic could be improved to make the application safer, more maintainable, and easier to review. For this enhancement, I added a more controlled database query layer that validates fields, limits accepted operators, applies projections, controls result limits, and improves database error handling.

This enhancement demonstrates my ability to improve database interaction in a way that supports security, reliability, and maintainability.

## What Was Improved

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

The original version allowed database logic to be handled more directly inside the database access class. The enhanced version separates query validation and database communication into clearer responsibilities.

## Files Involved

The main files related to this enhancement include:

- `database_query_service.py`: validates query fields, operators, projections, updates, and limits
- `animal_shelter.py`: uses the query service to perform safer MongoDB operations
- `config.py`: stores database configuration using environment variable support
- `dashboard_controller.py`: coordinates application requests with the database layer
- `app.py`: demonstrates database review mode output
- `.env.example`: documents expected environment variable configuration without exposing real credentials

## Skills Demonstrated

This enhancement showcases database design and security skills by improving how the application communicates with MongoDB. I added validation so that only approved fields and operators are used when building queries. I also added projection handling so the application can control which fields are returned from the database.

The enhancement also supports a stronger security mindset. Database credentials are not hard-coded into the enhanced source code. Instead, configuration values can be supplied through environment variables. This makes the project safer to publish, easier to configure, and more professional for review.

## Course Outcome Alignment

This enhancement supports the following CS 499 course outcomes:

- **Course Outcome 1:** Supports decision-making by improving how database records are retrieved and controlled for application use.
- **Course Outcome 2:** Demonstrates professional communication through clear documentation, code organization, and this enhancement writeup.
- **Course Outcome 3:** Supports thoughtful design choices involving database query construction, validation, limits, and tradeoffs.
- **Course Outcome 4:** Demonstrates the use of computing tools and techniques by improving the MongoDB access layer and separating database responsibilities.
- **Course Outcome 5:** Supports a security mindset through safer query validation, environment-based configuration, result limits, projections, and controlled database error handling.

## GitHub Repository

The code for this enhancement is available here:

[View Enhancement Three Code Repository](https://github.com/edward-mccauley/CS499-Grazioso-Salvare-ePortfolio)

## Return to Home

[Return to ePortfolio Home](https://edward-mccauley.github.io)
