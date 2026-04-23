🚀 Setup

Database

This project requires a running PostgreSQL instance on port 5432 with the following database:

* Name: study_feedback
* User: postgres
* Password: postgres

If you prefer different credentials, update them locally in application.yml (do not commit changes).

⸻

PostgreSQL Setup (Quick Guide)

1. Install PostgreSQL (any recent version works).
2. During setup:
    * Keep default port (5432)
    * Set password for postgres
    * Install pgAdmin
3. Open pgAdmin and connect to your server.
4. Create a database named study_feedback.

⸻

Running the App

Enable the local profile in your IntelliJ run configuration before starting the app.

⸻

🔧 Workflow

Git Strategy

We follow a feature branch workflow:

* Create branches from main
* Do not rebase before merging
* Resolve conflicts by merging main into your branch

Naming:
<issue-number>-<short-description> (e.g., 68-code-conventions)

Commit format:
project#<issue-number> - short description

⸻

Typical Workflow

1. Pull latest main
2. Create feature branch
3. Implement changes
4. Commit with proper message
5. Push branch
6. Open merge request
7. Get review → merge into main

⸻

🧑‍💻 Code Guidelines

General

* Prefer DTOs over entities in controllers (use MapStruct)
* Use Lombok to reduce boilerplate
* Format code and review changes before committing

⸻

Linting

Use SonarLint:

* Review all issues
* Fix all Critical and Blocker problems