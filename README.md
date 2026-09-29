
# Student Performance Tracker and Academic Risk Predictor

## 📌 About the Project

The **Student Performance Tracker and Academic Risk Predictor** is a Python-based project designed to help students and teachers understand academic performance in a simple and structured way.

The system takes a student's **name, attendance percentage, and marks in Maths, Science, and English** as input. It then calculates the student's total marks, average marks, assigns a grade, and predicts an academic risk level based on marks and attendance.

The project also provides a simple study suggestion according to the student's performance.

---

## 🎯 Objectives

The main objectives of this project are:

- To calculate a student's overall academic performance.
- To calculate total and average marks.
- To assign a grade based on average marks.
- To consider attendance while evaluating academic risk.
- To identify students who may need academic improvement.
- To provide a simple suggestion based on the student's performance.
- To prevent incorrect inputs through input validation.

---

## ✨ Features

### 1. Student Information
The program accepts:
- Student name
- Attendance percentage
- Maths marks
- Science marks
- English marks

### 2. Performance Calculation

The system calculates:

- **Total Marks**
- **Average Marks**
- **Grade**

The grading system used is:

| Average Marks | Grade |
|---|---|
| 90 – 100 | A+ |
| 75 – 89.99 | A |
| 60 – 74.99 | B |
| 50 – 59.99 | C |
| 40 – 49.99 | D |
| Below 40 | Fail |

### 3. Academic Risk Prediction

The system uses both **average marks and attendance** to determine academic risk.

| Condition | Risk Status |
|---|---|
| Average below 40 OR attendance below 50% | High Risk |
| Average below 60 OR attendance below 75% | Medium Risk |
| Otherwise | Low Risk |

### 4. Study Suggestions

Depending on the risk level, the system provides a suggestion:

- **High Risk:** Meet your teacher and focus on studies immediately.
- **Medium Risk:** Improve attendance and practise weak subjects.
- **Low Risk:** Keep up the good work.

### 5. Input Validation

The program checks for invalid inputs such as:

- Empty student names
- Non-numeric values
- Marks below 0
- Marks above 100
- Attendance below 0%
- Attendance above 100%

This helps prevent incorrect data from being processed.

---

## 🛠️ Technologies Used

- **Python**
- **Jupyter Notebook**
- **Python 3**

---

## 📂 Project Structure

```text
student-performance-tracker/
│
├── README.md
├── Student_Performance_Tracker.ipynb
└── statement.md
```

### File Description

**Student_Performance_Tracker.ipynb**  
Contains the Python code for collecting student information, calculating performance, assigning grades, predicting academic risk, validating inputs, and generating suggestions.

**statement.md**  
Contains the problem statement, project scope, target users, features, and technologies used.

**README.md**  
Contains the documentation and information about the project.

---

## 🚀 How to Run the Project

### Method 1: Using Jupyter Notebook

1. Install Python on your computer.
2. Install Jupyter Notebook if it is not already installed.
3. Download or clone this repository.
4. Open `Student_Performance_Tracker.ipynb`.
5. Run the notebook cells.
6. Enter the student's details when prompted.

### Method 2: Using Google Colab

1. Open Google Colab.
2. Upload `Student_Performance_Tracker.ipynb`.
3. Run the notebook cells.
4. Enter the requested student information.

---

## 💻 Example

### Input

```text
Enter student name: Ananya
Enter attendance percentage: 90
Enter Maths marks out of 100: 85
Enter Science marks out of 100: 88
Enter English marks out of 100: 92
```

### Output

```text
--- Performance Result ---

Student Name: Ananya
Total Marks: 265
Average Marks: 88.33
Grade: A

--- Risk Prediction ---

Risk Status: Low Risk
Suggestion: Keep up the good work.
```

---

## 🔍 How the System Works

The project follows these basic steps:

```text
        Start
          ↓
   Enter Student Name
          ↓
    Enter Attendance
          ↓
   Enter Subject Marks
          ↓
    Validate Inputs
          ↓
    Calculate Total
          ↓
   Calculate Average
          ↓
     Assign Grade
          ↓
   Predict Risk Level
          ↓
 Generate Study Suggestion
          ↓
         End
```

---

## 📊 Risk Prediction Logic

The project considers both academic marks and attendance.

```python
if average < 40 or attendance < 50:
    risk = "High Risk"

elif average < 60 or attendance < 75:
    risk = "Medium Risk"

else:
    risk = "Low Risk"
```

This provides a simple way to identify students who may require additional academic attention.

---

## 🧪 Input Validation

The program includes validation to make sure that the entered data is within the expected range.

For example:

```text
Marks: 400

Output:
Please enter a value between 0 and 100
```

If a user enters text instead of a number:

```text
Attendance: abc

Output:
Invalid input. Enter numbers only.
```

The program also prevents an empty student name from being accepted.

---

## 👥 Target Users

This project can be useful for:

- 🎓 Students who want to understand their academic performance.
- 👩‍🏫 Teachers who want a simple way to review student progress.
- 📚 Beginners learning Python and basic data-processing concepts.

---

## 🔮 Future Improvements

The project can be expanded in the future by adding:

- Multiple student records
- More subjects
- Graphs and performance charts
- Subject-wise performance analysis
- Student database storage
- Attendance history
- Login system
- A graphical user interface (GUI)
- Web-based dashboard
- Exporting performance reports
- More advanced academic risk prediction using machine learning

---

## 📚 Learning Outcomes

Through this project, the following concepts are demonstrated:

- Python input and output
- Variables and data types
- Arithmetic calculations
- Conditional statements
- Functions
- Loops
- Exception handling
- Input validation
- Basic academic data analysis
- Logical decision-making

---

## 📜 Project Scope

The current version focuses on a single student's:

- Name
- Attendance
- Maths marks
- Science marks
- English marks

It calculates performance and provides an academic risk status and suggestion based on the entered information.

---

## 👩‍💻 Author

**Tanisha Devdaliya**

GitHub: [Tanisha1709](https://github.com/Tanisha1709)

---

## ⭐ Conclusion

The **Student Performance Tracker and Academic Risk Predictor** demonstrates how Python can be used to process student information and provide meaningful academic feedback.

The project combines **performance calculation, grading, attendance analysis, risk prediction, and input validation** into a simple and beginner-friendly system.
