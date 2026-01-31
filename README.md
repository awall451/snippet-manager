# Dev Snippet Manager

A beginner-friendly Python application that stores and manages development-related snippets using an embedded SQLite database.

This project is designed as a learning exercise to practice:

- Python programming fundamentals  
- SQL and SQLite  
- Building a real-world CRUD application  
- Designing a project that can later grow into a full web application  

---

## Project Overview

The Dev Snippet Manager is a simple tool that allows developers to store, search, and manage useful code snippets such as:

- Bash commands  
- Docker commands  
- Kubernetes commands  
- SQL queries  
- Configuration fragments  

The application will begin as a command-line interface (CLI) tool and will eventually evolve into a web-based application with a TypeScript frontend.

---

## Goals

### Primary Learning Goals

- Learn how to interact with SQLite from Python  
- Understand basic database design  
- Implement Create, Read, Update, Delete (CRUD) operations  
- Organize a small Python project into modules  
- Practice working with SQL queries  

### Functional Goals

The application should allow a user to:

- Add new snippets  
- List all snippets  
- Search snippets by text or tags  
- View a specific snippet  
- Delete snippets  
- Update existing snippets  

---

## Technology Stack

Initial stack:

- Python 3  
- SQLite (embedded database)  
- Standard Python libraries  

Future stack:

- Flask or FastAPI backend  
- TypeScript frontend  
- Docker containerization  
- Kubernetes deployment  

---

## Data Model

### SQLite Schema (v1)

The core of the application will be a single table:

**snippets**

| Column      | Type    | Description                       |
|-------------|---------|-----------------------------------|
| id          | INTEGER | Primary Key                       |
| title       | TEXT    | Short name of the snippet         |
| content     | TEXT    | The actual snippet text           |
| language    | TEXT    | e.g. bash, python, sql            |
| tags        | TEXT    | Comma-separated tags              |
| created_at  | TEXT    | Timestamp when created            |
| updated_at  | TEXT    | Timestamp when last updated       |

---

## Project Structure

Initial project layout:
```bash
dev-snippet-manager/
│
├── snippets.py # Main CLI application
├── db.py # Database helper functions
├── schema.sql # SQLite table creation script
├── README.md # Project documentation
└── snippets.db # SQLite database (generated)
```

---

## Application Features (Planned)

### CLI Commands

The application will support commands such as:

```bash
python snippets.py add
python snippets.py list
python snippets.py search "kubernetes"
python snippets.py show 5
python snippets.py delete 5
```

---

## Development Phases

### Phase 1 – Basic Foundation

**Goals:**

- Create SQLite database  
- Define initial schema  
- Build simple Python script to connect to DB  

**Tasks:**

- Create `schema.sql`  
- Implement database initialization  # Dev Snippet Manager

A beginner-friendly Python application that stores and manages development-related snippets using an embedded SQLite database.

This project is designed as a learning exercise to practice:

- Python programming fundamentals  
- SQL and SQLite  
- Building a real-world CRUD application  
- Designing a project that can later grow into a full web application  

---

### Phase 2 – Core CLI Functionality

**Goals:**

- Implement basic CRUD operations  

**Tasks:**

- Add new snippets  
- List all snippets  
- View snippet by ID  
- Delete snippet  

---

### Phase 3 – Search and Organization

**Goals:**

- Improve usability  

**Tasks:**

- Implement text search  
- Add tag filtering  
- Improve CLI interface  

---

### Phase 4 – Code Cleanup and Structure

**Goals:**

- Improve project quality  

**Tasks:**

- Refactor into modules  
- Add error handling  
- Improve input validation  

---

### Phase 5 – Future Enhancements

Planned future improvements:

- Convert to a web application using Flask or FastAPI  
- Add a TypeScript frontend  
- Dockerize the application  
- Add user authentication  
- Add import/export functionality  

---

## Long-Term Vision

This project is intentionally designed to grow over time:

1. Start as a simple Python + SQLite CLI tool  
2. Evolve into a local web application  
3. Add a modern TypeScript frontend  
4. Become a containerized, deployable service  

---

## Getting Started (Future)

Instructions for running the application will be added as the project progresses.

---

## Purpose of This Project

This project exists primarily as a learning exercise. It is meant to be:

- Simple  
- Practical  
- Expandable  
- Realistic  
- Beginner-friendly  

By the end of this project, the goal is to have a solid understanding of how Python applications interact with databases and how small tools can grow into full applications.

---

## Author

Created as a personal learning project to explore Python, SQL, and application development.
- Write basic DB connection logic  
