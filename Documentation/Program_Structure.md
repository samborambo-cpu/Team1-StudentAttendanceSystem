# Program Structure – Student Attendance System

This document lists the major functions that will be developed when coding
begins (Assignment 3 and beyond). **No code is written at this stage** — this is
the planned structure only, as required by Section 2 (Project Design).

## Data design

Each of the (minimum) 25 student records will store three fields:

| Field | Type | Description |
|-------|------|-------------|
| Student ID | text / number | Unique identifier for the student |
| Student Name | text | Full name of the student |
| Attendance Status | text | One of: `Present`, `Absent`, `Late` |

Records will be held in a Python **list of dictionaries**, for example:

```
students = [
    {"id": "1001", "name": "Jane Doe", "status": "Present"},
    ...
]
```

## Major functions

| Function | Purpose |
|----------|---------|
| `main()` | Creates and maintains the students list and pass it to other functions as needed. |
| `display_menu()` | Prints the six menu options to the screen. |
| `add_record()` | Asks for Student ID, Name, and Status and adds a new record. |
| `search_record()` | Asks for a Student ID and displays that student's record (or "Not Found"). |
| `display_records()` | Displays all student records in a readable list/table. |
| `update_status()` | Finds a record by Student ID and updates its attendance status. |
| `generate_report()` | Calculates and displays the summary report. |
| `exit_program()` | Ends the program. |

### Planned function signatures (for future implementation)

```
def main():
    ...

def display_menu():
    ...

def add_record(students):
    ...

def search_record(students):
    ...

def display_records(students):
    ...

def update_status(students):
    ...

def generate_report(students):
    ...
```

## Menu options mapped to functions

| Menu # | Option | Function |
|--------|--------|----------|
| 1 | Add Record | `add_record()` |
| 2 | Search Record | `search_record()` |
| 3 | Display All Records | `display_records()` |
| 4 | Update Record Status | `update_status()` |
| 5 | Generate Summary Report | `generate_report()` |
| 6 | Exit Program | `exit_program()` |

## Summary report contents

The `generate_report()` function will display four reporting items:

1. **Total Students** – count of all records.
2. **Present Students** – count of records with status `Present`.
3. **Absent Students** – count of records with status `Absent`.
4. **Late Students** – count of records with status `Late`.
