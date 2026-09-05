# Student Record Management System — Project Report

## 1. Introduction
The Student Record Management System is a command-line application developed in Rust. Its purpose is to keep student information organized and allow the user to add, search, update, delete, and display student records. Records can also be saved to and loaded from a text file.

## 2. Objectives
- Practice Rust variables and data types.
- Use functions to divide the program into manageable parts.
- Use structs to represent student records.
- Practice ownership and borrowing.
- Use vectors to store multiple students.
- Use strings for names and departments.
- Use pattern matching for menu choices and result handling.
- Handle errors with `Result` and validation.
- Use modules to organize the program.
- Perform file input/output.
- Practice iterators for searching and filtering.
- Write basic automated tests.

## 3. Student Information
Each student record contains:
- Student ID
- Name
- Department
- Semester
- Marks
- Grade (calculated by the program)
- Pass/Fail status (calculated by the program)

## 4. Main Features
1. Add Student
2. Display Students
3. Search Student
4. Update Student
5. Delete Student
6. Search by Department
7. Show Result
8. Save Records
9. Load Records
10. Exit

## 5. Rust Concepts Used
### Variables and Data Types
The program uses integers for IDs and semesters, floating-point numbers for marks, and `String` for names and departments.

### Functions
Separate functions are used for adding, displaying, searching, updating, deleting, saving, and loading records.

### Structs
The `Student` struct groups related student information into one data type.

### Enums and Pattern Matching
The `match` expression in `main.rs` selects the correct operation according to the menu choice. Rust's `Result` type is also used for operations that can fail.

### Vectors
A `Vec<Student>` stores all student records while the program is running.

### Ownership and Borrowing
Functions borrow the student vector when they only need to read it and use mutable borrowing when records must be changed.

### Error Handling
The program validates IDs, semesters, marks, duplicate IDs, and file operations. Invalid input does not crash the program.

### Modules
The code is divided into `main.rs`, `student.rs`, `menu.rs`, and `file_manager.rs`.

### File Handling
Student records are saved in `students.txt` and loaded when requested.

### Iterators
Methods such as `find`, `filter`, and `position` are used to search and manipulate records.

### Testing
The `student.rs` module contains tests for grade calculation and invalid marks.

## 6. Example
A student can be entered as:
- ID: 101
- Name: Ali
- Department: Computer Science
- Semester: 4
- Marks: 78

The program calculates the grade as B+ and displays the student's result.

## 7. Expected Result
The final program provides a working terminal-based student record system. It demonstrates several important Rust concepts in one practical project without requiring a database or graphical interface.

## 8. Future Improvements
Possible future additions include sorting students, calculating class averages, importing records from another file, and adding more advanced functionality.

## 9. Conclusion
This project provides practical experience with Rust programming while solving a simple real-world record-management problem. It combines basic and intermediate Rust concepts in one application.
