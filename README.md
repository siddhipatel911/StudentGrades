# Student Grades 🧮📋

## Overview
**Student Grades** is a Java Swing GUI app that stores multiple students and their four course marks using a **2D array**.  
You can add students, list all stored records, compute **course averages** across the class, and compute a specific **student’s average** by name.  
All results are displayed in an on-screen text area.

- **Language:** Java
- **IDE:** NetBeans
- **GUI Library:** Java Swing
- **Status:** Complete

---

## Features

### ➕ Add Student
- Enter **First Name**, **Last Name**, and **four course marks** (percent).
- Click **Add** to append the record to a resizable `String[][]` (creates a new array with one extra row and copies existing data).

### 📄 List All
- Click **List** to display every stored student in the text area:
```text
First Last ---- C1: 78% C2: 84% C3: 91% C4: 88%
```

### 👤 Student Average
- Click **Student Average**, enter a **first and last name**, and the program calculates and shows **that student’s average** (out of the four courses).

### 🏫 Course Average
- Click **Course Average** to compute and print the **class average for each course** (Course 1–4).

### 🚪 Exit
- Closes the application.

---

## How It Works (Technical)
- Stores data in a **2D array**: each row = one student; columns = First, Last, Course1, Course2, Course3, Course4.
- **Dynamic growth**: on Add, creates a new array with `length + 1`, copies rows, and inserts the new student.
- Uses Swing **event listeners** on buttons to:
- Parse numeric inputs for averages
- Traverse rows to build the output in a `StringBuilder`
- Format averages to **two decimals**
- Displays output in a **multiline text area**.

---

## How to Run

### Option 1 — NetBeans (recommended)
1. Open NetBeans  
2. **File → Open Project…**  
3. Select the `StudentGrades` project folder (with `/src`, `/nbproject`, etc.)  
4. Run the project

Main class:
```java
studentgrades.StudentGrades
```

### Option 2: Run in Terminal
```bash
# clone the repo
git clone https://github.com/siddhipatel911/StudentGrades.git
cd StudentGrades/src

# compile
javac studentgrades/*.java

# run
java studentgrades.StudentGrades
```

---

## Example Output (snippets)
