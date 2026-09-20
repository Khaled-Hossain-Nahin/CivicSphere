# Smart Community Problem Reporting & Management System

A Java desktop application for reporting, assigning, and tracking local community problems, built as an Object-Oriented Programming (OOP) course project.

## Overview

The Smart Community Problem Reporting & Management System is a Java-based application that lets people report problems in their local area and follow what happens to those reports. It is meant to work for cities, towns, villages, and rural communities, not just urban areas.

The system connects three groups of users: citizens who report problems, officers who work on them, and an admin who coordinates everything. The application uses a Java Swing GUI and a database for storing data, and it is built to show how OOP principles apply in a real-world style project.

## Problem Statement

In many communities, reporting a local problem is harder than it should be. A broken streetlight or a leaking water pipe might be reported by phone, in person, or through a neighbor, and there is often no clear way to know whether anyone has looked at it. Complaints get lost, are handled late, or are never followed up on.

This is especially true in smaller towns and rural areas, where formal reporting channels are limited. This project tries to address that with a simple, structured system: one place to submit a problem, assign it to the right person, and see its progress.

## Project Objectives

- Give citizens an easy way to report local problems and check their status.
- Give administrators a central place to review, organize, and assign complaints.
- Let officers see the complaints assigned to them and record what was done.
- Make the process more transparent by keeping a clear status for every complaint.
- Apply core OOP concepts (encapsulation, inheritance, polymorphism, abstraction, interfaces, and exception handling) in a practical project.
- Design the system so it is not limited to urban use cases.

## Key Features

- User registration and login
- Complaint submission with category, description, and location
- Complaint status tracking for citizens
- Officer view of assigned complaints, with status updates and resolution notes
- Admin tools for managing users, complaints, and categories
- Assigning complaints to officers
- Desktop GUI built with Java Swing
- Database storage for users and complaints

## User Roles

| Role | What they can do |
|------|------------------|
| **Citizen** | Register and log in, submit a complaint, choose a category, add a description and location, track the status of their complaints |
| **Officer** | View complaints assigned to them, review the details, update the status, add resolution information, mark complaints as resolved |
| **Admin** | Manage citizen and officer accounts, view all complaints, assign complaints to officers, manage complaint categories, monitor the overall system |

## How the System Works

A typical complaint goes through these steps:

1. **Citizen reports a problem.** They pick a category, describe the issue, and add the location.
2. **Admin reviews the complaint.** The admin checks the details and decides who should handle it.
3. **Complaint is assigned to an officer.** The admin assigns it to a suitable officer.
4. **Officer works on it.** The officer reviews the complaint and updates its status as work progresses.
5. **Complaint is resolved.** The officer adds resolution information and marks it as resolved.
6. **Citizen tracks progress.** At any point, the citizen can log in and see the current status.

```
Citizen  →  Admin  →  Officer  →  Status updated  →  Citizen tracks progress
(report)   (review)   (assigned)    (in progress /     (view status)
                                      resolved)
```

## Problem Categories

The system starts with these categories. The admin can manage categories, so the list is not fixed.

| Category | Examples |
|----------|----------|
| Roads | Potholes, damaged or broken roads |
| Street Lighting | Broken or non-working streetlights |
| Waste Management | Uncollected garbage, illegal dumping |
| Drainage | Blocked drains, waterlogging |
| Water Supply | Pipe leaks, water supply issues |
| Electrical | Loose wires, faulty electrical equipment |
| Other | Any other local or community problem |

## OOP Concepts Used

This project is designed around the main OOP concepts. The class names below show how each concept is meant to be applied and may change as development continues.

| Concept | How it is applied |
|---------|-------------------|
| **Classes and Objects** | Core entities such as `User`, `Complaint`, and `Category` are modeled as classes, and each real user or complaint is an object. |
| **Encapsulation** | Fields are kept `private` and accessed through getters and setters, so data such as complaint status is only changed through controlled methods. |
| **Inheritance** | `Citizen`, `Officer`, and `Admin` extend a common `User` class and share fields like name, email, and password. |
| **Polymorphism** | Overridden methods (for example, a role-specific menu or dashboard method) behave differently depending on the type of user. Method overloading is used where a method needs multiple input forms. |
| **Abstraction** | `User` is an abstract class that defines what every user has and does, without being created directly. |
| **Interfaces** | Interfaces define shared behavior, for example, actions that only certain roles can perform (such as a complaint-management interface). |
| **Constructors** | Constructors initialize objects with valid starting data, such as a new complaint starting with a "Pending" status. |
| **Collections** | Lists (such as `ArrayList`) are used to hold groups of objects like complaints and users. |
| **Exception Handling** | `try-catch` blocks and custom exceptions handle problems such as invalid login, empty input, or database errors. |

## Technologies Used

| Technology | Purpose |
|------------|---------|
| Java | Main programming language |
| Java Swing | Graphical user interface |
| Database | Storing users, complaints, and categories |
| NetBeans IDE | Development environment |
| Git & GitHub | Version control and code hosting |

## Project Scope

**Included in this project:**

- Three user roles: citizen, officer, and admin
- Submitting, assigning, and tracking complaints
- Category management by the admin
- A desktop application with a Swing interface

**Not included (for now):**

- Web or mobile versions
- Live map integration or GPS location
- Automatic notifications (email or SMS)
- Photo uploads with complaints

## Future Improvements

These are ideas for the future, not part of the current work:

- Photo attachments for complaints
- Map or GPS-based location selection
- Email or SMS notifications when a status changes
- Complaint priority levels (for example, urgent or normal)
- Search and filter options for the admin
- Reports and statistics on complaints by category or area
- A web or mobile version so more people can use it
- Support for multiple languages, which would help in rural and local communities

## Contributors
| Contributor Name | Student ID |
|----------|----------|
| Khaled Hossain | 252-15-026 |
| Elora Akcha | 252-15-558 |
| Soyaiba Rahman | 252-15-678 |
| Jaoyata Afnan | 252-15-529 |
| Jaoyata Afnan | 252-15-139 |
