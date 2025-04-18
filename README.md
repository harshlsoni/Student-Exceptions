
# 🎓 Student Management System (with Custom Exceptions)

This Java-based console application allows users to manage student data including adding, displaying, updating, searching, and deleting student records. It demonstrates the use of **custom exceptions** to handle duplicate entries and missing student records gracefully.

---

## ✨ Features

- ➕ Add new student  
- 📋 Display all students  
- 🔍 Search student by:
  - PRN
  - Name
  - Position (index)
- ✏️ Update student details  
- ❌ Delete student  
- 🚫 Custom exceptions:
  - `DuplicateStudentException` for duplicate PRN
  - `StudentNotFoundException` for invalid search/update/delete

---

## 🧱 Project Structure

- `Student.java` – Represents a student with attributes: PRN, Name, DOB, Marks.
- `StudentManager.java` – Core class to handle all student-related operations.
- `Main.java` – Entry point with a menu-driven interface.
- `exceptions/DuplicateStudentException.java` – Custom exception for duplicate entries.
- `exceptions/StudentNotFoundException.java` – Custom exception for missing students.

---

## 🛠️ How to Run

1. **Clone the Repository**
   ```bash
   git clone https://github.com/harshlsoni/Student-Exceptions
   cd Student-Exceptions
   ```

2. **Compile the Project**
   Ensure your directory structure maintains the `exceptions` package.
   ```bash
   javac exceptions/*.java *.java
   ```

3. **Run the Program**
   ```bash
   java Main
   ```

---

## 🧪 Sample Menu Output

```
===== Student Data Entry System =====
1. Add Student
2. Display All Students
3. Search Student
4. Update Student
5. Delete Student
0. Exit
Enter your choice:
```

---

## 🚨 Exception Handling Example

- Adding a student with an existing PRN:
  ```
  Error: Student with PRN already exists!
  ```
- Searching for a student that doesn't exist:
  ```
  Error: PRN not found.
  ```

