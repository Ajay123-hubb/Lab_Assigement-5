# Student Record Management System — Java (OOP + File Handling + Exceptions + Multithreading + Collections)

## 📖 Overview
This project implements a complete **Student Record Management System** in Java.  
It uses **Object-Oriented Programming (OOP)**, **Java Collections API**, **Exception Handling**, **Multithreading**, and **File I/O**.

The system supports:
- Adding student records
- Updating student marks
- Deleting student records
- Searching by Roll No
- Viewing all students
- Sorting by marks
- Persistent file storage

All student data is stored in `students.txt`.

---

## 🎯 Learning Outcomes
According to the lab assignment: :contentReference[oaicite:1]{index=1}

✔ Apply **abstraction, inheritance, interfaces**  
✔ Handle invalid input using **custom exceptions & try-catch**  
✔ Load & save records using **file handling**  
✔ Manage records using **List & Map Collections**  
✔ Implement **Comparator sorting** for marks  
✔ Use **Iterator** for displaying records  
✔ Simulate loading via **multithreading (Runnable / Thread)**  
✔ Follow **modular design**

---

## 🧠 Core Concepts Implemented

### 🔹 1. Abstraction
`Person` is an **abstract class**
- Fields: `name`, `email`
- Abstract Method: `displayInfo()`

### 🔹 2. Inheritance
`Student` **extends Person**
- Adds: `rollNo`, `course`, `marks`, `grade`
- Methods:
  - `calculateGrade()`
  - `displayDetails()`

### 🔹 3. Interfaces
`RecordActions` includes:
- `addStudent()`
- `updateStudent()`
- `deleteStudent()`
- `searchStudent()`
- `viewAllStudents()`

Implemented in `StudentManager`.

### 🔹 4. Collections
- `List<Student>` → store records
- `Map<Integer, Student>` → fast rollNo lookup

### 🔹 5. Sorting
Sorts by marks (HIGH → LOW) using:
```java
Comparator<Student>
