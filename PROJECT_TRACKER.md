# Dental Clinic Management System — Development Tracker

## EPIC-01: Foundation

**Workflow:** Backlog → Ready → In Progress → In Review → Testing → Done

| ID | Task | Priority | Status |
|---|---|---|---|
| TASK-01 | Create repository and project structure | P0 | Todo |
| TASK-02 | Define environments | P0 | Todo |
| TASK-03 | Create PostgreSQL development database | P0 | Todo |
| TASK-04 | Define initial domain model | P0 | Todo |
| TASK-05 | Create ERD | P0 | Todo |
| TASK-06 | Implement authentication/RBAC foundation | P0 | Todo |
| TASK-07 | Implement Patient module | P0 | Todo |
| TASK-08 | Implement Appointment module | P0 | Todo |
| TASK-09 | Connect Patient → Appointment workflow | P0 | Todo |
| TASK-10 | Add automated tests | P0 | Todo |

## TASK-01 — Create repository and project structure

### Objective
Establish the initial repository structure for the Dental Clinic Management System.

### Acceptance criteria
- Clear, maintainable project structure.
- Application can be installed and started from documented instructions.
- No secrets are committed.
- README documents local setup and development workflow.

## TASK-02 — Define environments

### Objective
Define development, testing, and production environment conventions.

### Acceptance criteria
- Required configuration variables are documented.
- Secrets are excluded from Git.
- Local environment can be created from a safe template.
- Environment responsibilities are documented.

## TASK-03 — Create PostgreSQL development database

### Objective
Create the PostgreSQL development database foundation.

### Acceptance criteria
- Backend connects successfully to PostgreSQL.
- Database configuration is environment-based.
- Initial migration/schema workflow is repeatable.
- Database credentials are not committed.

## TASK-04 — Define initial domain model

### Objective
Define the initial domain model for the first vertical slice.

### Core entities
- User / Role
- Patient
- Appointment

### Acceptance criteria
- Entities, fields, constraints, and relationships are documented.
- Model supports the Patient → Appointment workflow.
- Design decisions are documented before implementation.

## TASK-05 — Create ERD

### Objective
Create the Entity Relationship Diagram for the initial database model.

### Acceptance criteria
- ERD is committed to the repository.
- Primary keys, foreign keys, cardinality, and important constraints are represented.
- Patient → Appointment relationship is clear.
- ERD stays aligned with the database schema.

## TASK-06 — Implement authentication/RBAC foundation

### Objective
Implement authentication and role-based access control.

### Acceptance criteria
- Users can authenticate.
- Protected resources reject unauthenticated access.
- Role checks restrict protected operations.
- Critical authentication/authorization paths are tested.

## TASK-07 — Implement Patient module

### Objective
Implement the initial Patient management module.

### Acceptance criteria
- Authorized users can create patients.
- Authorized users can view patient information.
- Authorized users can update patient information.
- Required-field validation works.
- Critical patient operations are tested.

## TASK-08 — Implement Appointment module

### Objective
Implement the initial Appointment module.

### Acceptance criteria
- Authorized users can create appointments for patients.
- Appointment details can be viewed and updated.
- Invalid appointment data is rejected.
- Patient association is enforced.
- Critical appointment operations are tested.

## TASK-09 — Connect Patient → Appointment workflow

### Objective
Complete the first end-to-end vertical slice.

### Acceptance criteria
- User can create/select a patient and create an appointment for that patient.
- Appointment references the correct patient.
- Relevant patient/appointment information is linked across UI, API, and database.
- Main success and failure paths are tested.

## TASK-10 — Add automated tests

### Objective
Establish automated coverage for the foundation and first vertical slice.

### Acceptance criteria
- Tests run through a documented command.
- Critical business rules have automated coverage.
- Patient and Appointment API behavior is tested.
- RBAC restrictions are tested.
- First vertical slice tests pass before completion.

## Definition of Done for the first vertical slice

- Database schema exists and migrations work.
- Authentication/RBAC foundation is functional.
- Patient CRUD works.
- Appointment CRUD works.
- Patient → Appointment workflow works end-to-end.
- Validation and authorization are enforced.
- Automated tests pass.
- Setup and architecture are documented.
