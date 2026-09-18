# Student Marks & Grade Management System

## Problem Statement

Managing student marks manually can be repetitive and error-prone. Manual calculations may lead to incorrect totals, percentages, or grades, while maintaining unstructured records can make it difficult to search, display, and manage student information.

The Student Marks & Grade Management System provides a simple console-based Java solution for managing student academic records. The system allows users to add, display, search, and delete student records, while automatically calculating total marks, percentage, and grade.

## Objectives

- Develop a practical Java application using CSE2006 concepts.
- Store and manage multiple student records using `ArrayList`.
- Accept and validate student details and marks.
- Calculate total marks, percentage, and grade automatically.
- Provide add, display, search, generate-result, and delete operations.
- Demonstrate Object-Oriented Programming concepts such as:
  - Classes and objects
  - Constructors
  - Encapsulation
  - Inheritance
  - Method overriding
  - Polymorphism
- Handle invalid inputs using exception handling.
- Demonstrate multithreading through a separate report-generation thread.

## Features

1. Add Student
2. Display All Students
3. Search Student by Roll Number
4. Generate Student Result
5. Delete Student
6. Input Validation
7. Exception Handling
8. Thread-based Report Generation

## Grade Calculation

| Percentage | Grade |
|---|---|
| 90 and above | A+ |
| 80–89.99 | A |
| 70–79.99 | B |
| 60–69.99 | C |
| 50–59.99 | D |
| 40–49.99 | E |
| Below 40 | F |

## Technologies Used

- Java
- ArrayList
- Object-Oriented Programming
- Exception Handling
- Multithreading
- Console-based User Interface

## Project Structure

```text
StudentMarksManagement/
├── Main.java
├── Person.java
├── Student.java
├── Marks.java
├── Result.java
├── StudentManager.java
├── InputValidator.java
└── ReportThread.java
