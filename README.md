# Departmental Dashboard (C++)

This is a small C++ project I made to practice object-oriented programming (OOP) concepts like classes, inheritance, and polymorphism. The program simulates a simple company dashboard with different teams (like Sales, Engineering, HR, etc.).

While this is a small-scale project, I focused on modeling a departmental dashboard as it might be used in an actual organization, managing teams across Marketing, Sales, Engineering, Human Resources, and Communications. The implementation showcases practical features such as team management, inter-department communication, and detailed team reporting, reflecting how these OOP concepts can be applied to real business scenarios.

- **Creates teams for different departments** (Sales, Engineering, HR, Communications, Marketing) using classes and inheritance.
- **Lets you add members, set budgets, and update locations** for each team.
- **Shows how polymorphism works** by letting teams communicate with each other using shared methods.
- **Prints out information** about each team, their members, and their budgets.
- **Demonstrates namespaces** by organizing code for each department.

## Example Output

When you run the program, you’ll see output like this:

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

And for communication between teams:

```
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

## Why did I make this?

I wanted to get better at using classes, inheritance, and namespaces in C++. This project helped me understand how to organize code for different parts of a program and how to use polymorphism for shared actions.

## How to Run

1. Make sure you have a C++ compiler (like g++) installed.
2. Compile the code:
   ```
   g++ src/mainDepartmentalDashboard.cpp -I include -o dashboard
   ```
3. Run the program:
   ```
   ./dashboard
   ```

## Author

Rodrigo Casio  
[My GitHub Profile](https://github.com/rodrigcasio)