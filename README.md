# 🎓 Student Record Management System (CLI Based)

A simple **Java CLI-based Student Record Management System** that supports basic **CRUD operations** (Create, Read, Update, Delete) using `ArrayList`.  
This project is built in **IntelliJ IDEA CE** as a part of learning Java fundamentals.

---

## 📌 Features
- ➕ Add a new student with ID, name, and marks.
- 📋 View all students.
- ✏️ Update existing student details using ID.
- ❌ Delete student by ID.
- 🖥️ Interactive **menu-driven CLI** system.

---

## 📌 Project Structure
![img.png](out/img.png)

---

- **Main.java** → Entry point of the program.
- **Student.java** → Model class representing student entity.
- **StudentManager.java** → Contains CRUD logic and menu system.

---

## 📌 Tools & Technologies
- ☕ Java 17+
- 🖥 IntelliJ IDEA Community Edition
- 📚 Java Collections (ArrayList, Scanner)

---

## 📌 How We Built the Project (Step by Step)

### 1. Understanding the Requirements
We had to build a CLI-based CRUD system where we can:
- Add student records
- View all students
- Update student details
- Delete student records

We also decided to use:
- `Student` class → to represent a student
- `ArrayList` → to store student objects dynamically
- `Scanner` → to take user input from console

---

### 2. Creating the `Student` Class
We started by making a **model class** called `Student` with 3 fields:
- `id` → unique identifier for student
- `name` → student’s name
- `marks` → student’s marks

We also added:
- **Constructor** to initialize objects
- **Getters/Setters** to modify fields
- **toString()** method to display student info

---

### 3. Writing the `StudentManager` Class
Next, we created a **service class** that handles all CRUD operations.  
It contains:
- An `ArrayList<Student>` to store records
- Methods:
    - `addStudent()` → to add a student
    - `viewStudents()` → to display all students
    - `updateStudent()` → to update a student by ID
    - `deleteStudent()` → to delete a student by ID

We also added a `start()` method with a **menu loop** that keeps running until user exits.

---

### 4. Setting up the `Main` Class
Finally, we created a **Main.java** file which acts as entry point.  
It simply calls:
```java
public static void main(String[] args) {
    StudentManagementSystem sms = new StudentManagementSystem();
    sms.start(); // starts menu-driven program
}

## 📌 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/YourUsername/student-management-system.git
