# Student Attendance System

**Team 1** — Introduction to Programming, Assignment 2

A console-based Python application that allows a school to track student
attendance for a class. It manages at least 25 student records and generates an
attendance summary report. *(No source code yet — this assignment covers planning,
design, and GitHub setup only.)*

🔗 **Repository:** https://github.com/samborambo-cpu/Team1-StudentAttendanceSystem

## Team Members
All members are **Software Developers**; each also holds a coordination role.
- **Samuel Azize** — Software Developer & Project Manager / GitHub Coordinator
- **Camilo Sequeira** — Software Developer & Documentation Manager
- **Luis Monsalve** — Software Developer & Design / Technical Lead

## Project Description
The Student Attendance System tracks attendance for a class of at least 25
students. Each record stores a **Student ID**, **Student Name**, and
**Attendance Status** (Present, Absent, or Late). Through a simple text menu, the
user can add records, search for a student, display all records, update a
student's status, and generate a summary report.

## Problem Statement
Taking attendance on paper is slow, easy to lose, and prone to human error.
Teachers need a fast, consistent way to record each student's status and instantly
see class totals. This system stores attendance digitally and generates an
accurate summary report on demand.

## Project Goals
- Add attendance records (ID, Name, Status)
- Search for a student record by ID
- Display all attendance records
- Update a student's attendance status
- Generate a summary report (Total, Present, Absent, Late)
- Provide a clear, menu-driven interface

## Assigned Roles
Every team member is a **Software Developer** and will contribute to the future
implementation. In addition, each member holds a coordination role:

| Member | Roles | Responsibilities |
|--------|-------|------------------|
| Samuel Azize | Software Developer & Project Manager / GitHub Coordinator | Contributes to development; coordinates the team, tracks progress, manages the repository and collaborators |
| Camilo Sequeira | Software Developer & Documentation Manager | Contributes to development; maintains documentation and organizes project files |
| Luis Monsalve | Software Developer & Design / Technical Lead | Contributes to development; owns the system design (flowchart, program structure) and leads technical decisions |

## System Flowchart
The full flowchart is in [`Flowcharts/attendance_flowchart.md`](Flowcharts/attendance_flowchart.md)
(rendered below) with an image version at `Flowcharts/attendance_flowchart.png`.

```mermaid
flowchart TD
    A([Start]) --> B[Load / Initialize<br/>Student Records]
    B --> C[Display Main Menu]
    C --> D[/Enter choice 1-6/]
    D --> E{Menu Choice}
    E -->|1 - Add Record| F[Add Record]
    E -->|2 - Search Record| G[Search Record]
    E -->|3 - Display Records| H[Display All Records]
    E -->|4 - Update Status| I[Update Status]
    E -->|5 - Summary Report| J[Generate Summary Report]
    E -->|6 - Exit| K([Exit Program])
    F --> C
    G --> C
    H --> C
    I --> C
    J --> C
```

## Repository Structure
| Folder | Contents |
|--------|----------|
| `Documentation/` | Project plan, program structure, team responsibilities, submission draft |
| `Flowcharts/` | System flowchart (Mermaid, PNG, and text versions) |
| `SourceCode/` | Reserved for future Python source code |
| `Screenshots/` | GitHub screenshots for the submission |
