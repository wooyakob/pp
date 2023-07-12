# pp
portfolio project
# Employee Manager API

## Description
The Employee Manager API is a RESTful service designed to manage employees, their respective departments, and project assignments within a company. It provides functionalities to create, read, update, and delete (CRUD) information about employees, departments, and projects. It also allows querying of employee assignments to projects.

## API Reference

| Endpoint | HTTP Method | Parameters | Description |
|---|---|---|---|
| `/employees` | GET | - | Fetch all employees |
| `/employees` | POST | `name`, `position`, `salary`, `department_id` | Create a new employee |
| `/employees/{employee_id}` | GET | `employee_id` | Fetch specific employee |
| `/employees/{employee_id}` | PUT | `employee_id`, `name`, `position`, `salary`, `department_id` | Update specific employee |
| `/employees/{employee_id}` | DELETE | `employee_id` | Delete specific employee |
| `/departments` | GET | - | Fetch all departments |

## Retrospective

### How did the project's design evolve over time?
The initial design of the API was quite simple, focusing on providing basic CRUD operations for employees. As the project evolved, we realized the need to manage not only employees but also the departments they work in and the projects they are assigned to. This led to the expansion of the API to include endpoints for departments and projects. 

### Did you choose to use an ORM or raw SQL? Why?
We chose to use an ORM (Object-Relational Mapping) for this project because ORMs reduce the amount of written SQL code, thus reducing potential syntax errors.

### What future improvements are in store, if any?
- Employee authentication and role-based access control
- Advanced querying capabilities (e.g., filter by department, search employees by name, etc.)
- Detailed logging and error handling mechanisms
