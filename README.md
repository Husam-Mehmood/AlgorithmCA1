# Employee Training Course Manager — Custom Linked List ADT

A Java console application for managing employees enrolled in training courses, built on top of a **singly-linked list implemented entirely from scratch** (no `java.util` collections) as an Abstract Data Type (ADT).

## What it demonstrates
- A generic `LinkedListADT<T>` interface and `LinkedList<T>` implementation using custom `LinearNode<T>` links — covers add-at-position, remove-by-match, size/isEmpty, and traversal.
- Domain logic layered on top of the ADT: an `Employee` class with validation rules (must have 5+ years of experience; course names must start with `"FOOD"`).
- A console-driven workflow (`TrainingCourses`) that:
  - Accepts up to 10 employees and inserts each at a user-chosen position in the list
  - Removes an employee by employee number
  - Bulk-removes all employees enrolled in a given course
  - Awards certifications to an employee by name + course
  - Displays the full employee list

## Tech stack
Java, custom data structures (no external libraries).

## Running it

```bash
javac -d bin src/util/*.java src/application/*.java
java -cp bin application.TrainingCourses
```

## Project background
Built as coursework for an Algorithms / Data Structures module, focused on implementing a linked list ADT from first principles and applying it to a realistic management scenario.
