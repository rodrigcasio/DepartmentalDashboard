# DepartmentalDashboard: C++ OOP Project

A C++ project designed to demonstrate object-oriented programming (OOP) principles—including polymorphism, encapsulation, and abstraction—in a context that simulates a real-world company environment. 

While this is a small-scale project, I focused on modeling a departmental dashboard as it might be used in an actual organization, managing teams across Marketing, Sales, Engineering, Human Resources, and Communications. The implementation showcases practical features such as team management, inter-department communication, and detailed team reporting, reflecting how these OOP concepts can be applied to real business scenarios.

## Features

- **Teams**: Each department (Marketing, Sales, Engineering, HR, Communications) has its own `Team` class, all inheriting from a common `DepartmentTeamBase` interface.
- **Namespaces**: Departments are organized using C++ namespaces for modularity and clarity.
- **Team Management**: Add members, set budgets, update locations, and print detailed team information for each department.
- **Polymorphic Communication**: Teams communicate with each other using a shared interface, demonstrating polymorphism via virtual functions.
- **Auditing**: Support namespaces (e.g., `Marketing::Support`) provide functions for auditing and inter-department messaging.

## OOP Principles

- **Polymorphism**: All `Team` classes inherit from `DepartmentTeamBase` and override the `getTeamName()` method, enabling generic functions like `communicateToDeparment()` to work with any team.
- **Encapsulation**: Team data (name, members, budget, location) is private and accessed via public methods.
- **Abstraction**: Common operations (e.g., printing team details, communication) are abstracted through base class interfaces and support functions.
- **Namespaces**: Each department and its support functions are encapsulated in their own namespace for clear separation of concerns.

## Purpose

Developed as part of my C++ learning journey to demonstrate mastery of OOP concepts, namespaces, and modular design. This project showcases my ability to design and implement extensible systems using inheritance, vectors, and polymorphism.

## Project Structure

- `src/` — Source files (e.g., `mainDepartmentalDashboard.cpp`)
- `include/` — Header files for each department and the base class

## How to Build

```bash
g++ src/mainDepartmentalDashboard.cpp -I include -o dashboard
./dashboard
```

## Sample Output

### Team Details
```
Sales Team Name: Stellar Corp-Sales
Location: London
Members: Pratik, Emily, Clive .
---
Engineering Team Name: Stellar Corp-Engineering
Location: Guadalajara
Budget: $900000
Team Members: Rodrigo, Luis, Alberto .
---
Human Resources Team Name: Stellar Corp-HR
Location: New Mexico
Budget: $50000
Members: Jonas, Sally, Penny .
---
Communications Team Name: Stellar Corp-Communications
Location: Chicago
Budget: $60000
Members: Paul, Stephen, Katy .
```

### Inter-Department Communication
```
---- Example of using the method communcatedToDepartment() ---
New message from: Stellar Corp-Marketing
To: Stellar Corp-Engineering
Message: "We need information about your upcoming project ASAP"
---
New message from: Stellar Corp-Engineering
To: Stellar Corp-HR
Message: "We need orientation for a new intern. Starting next week"
---
New message from: Stellar Corp-Communications
To: Stellar Corp-Sales
Message: "Need update of the current sales of the month, please."
```

### Auditing Example
```
Auditing Marketing Team: Stellar Corp-Marketing
Number of Members: 3
Team Budget: 500000
Audit complete
```

## Author

Rodrigo Casio ([View my Github profile](https://github.com/rodrigcasio))