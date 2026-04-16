# AI Workshop - OpenEdge ABL Project

This project demonstrates the OpenEdge ABL Business Entity Architecture Pattern with a complete example implementation.

## Project Structure

```
ProjectGengar/
|-- src/
|   |-- business/
|   |   |-- CustomerEntity.cls      # Business entity for Customer data
|   |   |-- EntityFactory.cls       # Singleton factory for entity management
|   |   |-- CustomerDataset.i       # Dataset definition for Customer entity
|   |-- CustomerWin.w              # Customer management UI window
|   |-- ItemWin.w                   # Item management UI window
|-- .windsurf/
|   |-- rules/                      # Development rules and guidelines
|   |-- workflows/                  # Automated workflows for common tasks
|-- .github/
|   |-- ISSUE_TEMPLATE/             # GitHub issue templates
|-- doc/
|   |-- business-entity-pattern.md  # Complete documentation of the architecture pattern
|-- dump/
|   |-- sports2000.df              # Sports2000 database schema
|-- openedge-project.json          # OpenEdge project configuration
|-- build.xml                      # Ant build configuration
```

## Architecture Overview

This project implements a layered architecture following the Business Entity pattern:

1. **UI Layer** - Windows and forms that handle user interaction
2. **Business Entity Layer** - Data access, validation, and business logic
3. **Database Layer** - Persistent storage (Sports2000 database)

### Key Components

- **EntityFactory**: Singleton pattern for managing business entity instances
- **CustomerEntity**: Business entity encapsulating all Customer data operations
- **CustomerDataset**: Temp-table and dataset definitions for data transfer
- **Business Entity Pattern**: Comprehensive documentation of the architecture

## Features

- Complete CRUD operations for Customer entity
- Validation framework with error handling
- Change tracking for updates
- Singleton factory pattern for entity management
- Comprehensive documentation and examples
- Automated workflows for common development tasks

## Getting Started

1. Clone this repository
2. Ensure you have OpenEdge 12.8 or later installed
3. Configure your database connection in `openedge-project.json`
4. Compile the project using the provided build configuration
5. Run the CustomerWin.w or ItemWin.w windows to interact with the application

## Documentation

See `doc/business-entity-pattern.md` for comprehensive documentation of the Business Entity Architecture Pattern, including:

- Step-by-step implementation guide
- Common pitfalls and solutions
- Refactoring legacy code
- Best practices and examples

## Development Tools

This project includes Windsurf workflows for common development tasks:

- `/newclass_example` - Create new ABL classes
- `/newconstructor` - Add constructors to classes
- `/newmethod_example` - Add methods to classes
- `/newproperty_example` - Add properties to classes

## Database

The project uses the Sports2000 sample database. The schema is available in `dump/sports2000.df`.

## License

This project is provided as an educational resource for learning OpenEdge ABL development patterns.